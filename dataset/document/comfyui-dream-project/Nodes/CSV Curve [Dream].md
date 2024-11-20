---
tags:
- AnimationScheduling
- Curve
---

# 📈 CSV Curve
## Documentation
- Class name: `CSV Curve [Dream]`
- Category: `✨ Dream/🎥 animation/📈 curves`
- Output node: `False`

The CSV Curve node is designed to interpret and apply animation curves based on data extracted from CSV files. It allows for the dynamic generation of animation parameters through the parsing of CSV file content, supporting interpolation and customization of the CSV parsing process.
## Input types
### Required
- **`frame_counter`**
    - A counter tracking the current frame of the animation, essential for timing and synchronization of the animation curve with the overall animation sequence.
    - Comfy dtype: `FRAME_COUNTER`
    - Python dtype: `FrameCounter`
- **`csvfile`**
    - Specifies the path to the CSV file to be used for generating the animation curve, enabling the node to dynamically interpret and apply the data contained within.
    - Comfy dtype: `STRING`
    - Python dtype: `str`
- **`first_column_type`**
    - Determines whether the first column of the CSV file represents seconds or frames, affecting how the data is interpreted in the context of animation timing.
    - Comfy dtype: `COMBO[STRING]`
    - Python dtype: `List[str]`
- **`interpolate`**
    - Controls whether interpolation is applied between data points in the CSV file, allowing for smoother transitions in the generated animation curve.
    - Comfy dtype: `COMBO[STRING]`
    - Python dtype: `List[str]`
- **`csv_dialect`**
    - Specifies the dialect of the CSV file, enabling the node to accurately parse files with different formatting conventions.
    - Comfy dtype: `COMBO[STRING]`
    - Python dtype: `List[str]`
## Output types
- **`FLOAT`**
    - Comfy dtype: `FLOAT`
    - The floating-point value generated by the CSV Curve node, representing a point on the animation curve.
    - Python dtype: `float`
- **`INT`**
    - Comfy dtype: `INT`
    - An integer representation of the generated animation curve point, providing an alternative precision level.
    - Python dtype: `int`
## Usage tips
- Infra type: `CPU`
- Common nodes: unknown


## Source code
```python
class DreamCSVCurve:
    NODE_NAME = "CSV Curve"

    @classmethod
    def INPUT_TYPES(cls):
        return {
            "required": SharedTypes.frame_counter | {
                "csvfile": ("STRING", {"default": "", "multiline": False}),
                "first_column_type": (["seconds", "frames"],),
                "interpolate": (["true", "false"],),
                "csv_dialect": (csv.list_dialects(),)
            },
        }

    CATEGORY = NodeCategories.ANIMATION_CURVES
    RETURN_TYPES = ("FLOAT", "INT")
    RETURN_NAMES = ("FLOAT", "INT")
    FUNCTION = "result"

    @classmethod
    def IS_CHANGED(cls, *values):
        return hashed_as_strings(*values)

    def _row_yield(self, file, csv_dialect):
        prev_row = None
        for row in csv.reader(file, dialect=csv_dialect):
            if len(row) == 2 and _is_as_float(row[0]) and _is_as_float(row[1]):
                row = list(map(float, row))
                yield (prev_row, row)
                prev_row = row
        if prev_row is not None:
            yield (prev_row, None)

    def result(self, csvfile, frame_counter: FrameCounter, first_column_type, interpolate, csv_dialect):
        interpolate = interpolate == "true"

        def _first_col_to_frame(v: float):
            if first_column_type == "frames":
                return round(v)
            else:
                return round(v * frame_counter.frames_per_second)

        with open(csvfile) as f:
            for (prev, current) in self._row_yield(f, csv_dialect):
                if prev is None and frame_counter.current_frame < _first_col_to_frame(current[0]):
                    # before first row
                    return (current[1], int(round(current[1])))
                if current is None:
                    # after last row
                    return (prev[1], int(round(prev[1])))
                if prev is not None and current is not None:
                    frame1 = _first_col_to_frame(prev[0])
                    value1 = prev[1]
                    frame2 = _first_col_to_frame(current[0])
                    value2 = current[1]
                    if frame1 <= frame_counter.current_frame and interpolate and frame2 > frame_counter.current_frame:
                        offset = (frame_counter.current_frame - frame1) / float(frame2 - frame1)
                        v = value1 * (1.0 - offset) + value2 * offset
                        return (v, int(round(v)))
                    elif frame1 <= frame_counter.current_frame and frame2 > frame_counter.current_frame:
                        return (value1, int(round(value1)))
        return (0.0, 0)

```