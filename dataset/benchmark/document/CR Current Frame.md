- `CR Current Frame`: The CR Current Frame node is designed to manage and optionally display the current frame index within an animation sequence. It allows for the adjustment of the frame index and provides an option to print the current frame index to the console, facilitating debugging and tracking of animation progress.
    - Inputs:
        - `index` (Required): Specifies the current frame index. It is crucial for determining the specific frame being processed or displayed in the animation sequence. Type should be `INT`.
        - `print_to_console` (Required): Determines whether the current frame index should be printed to the console. This is useful for debugging purposes and tracking the progress of the animation. Type should be `COMBO[STRING]`.
    - Outputs:
        - `index`: Returns the current frame index. This is essential for tracking the progress of the animation and for further processing of the specific frame. Type should be `INT`.
