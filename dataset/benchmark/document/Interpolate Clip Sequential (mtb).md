- `Interpolate Clip Sequential (mtb)`: This node is designed for sequential interpolation of text encodings within a given base text, using specified replacements and an interpolation strength parameter. It aims to modify the base text by interpolating new text encodings, thereby achieving a seamless transition between the original and the new text content.
    - Inputs:
        - `base_text` (Required): The original text content that serves as the starting point for interpolation. Type should be `STRING`.
        - `text_to_replace` (Required): The specific portion of the base text that is targeted for replacement through interpolation. Type should be `STRING`.
        - `clip` (Required): A parameter that influences the degree to which the original text is modified, controlling the blend between the original and new text encodings. Type should be `CLIP`.
        - `interpolation_strength` (Required): Defines the intensity of the interpolation effect, adjusting how prominently the new text encodings are integrated into the base text. Type should be `FLOAT`.
    - Outputs:
        - `conditioning`: The result of the interpolation process, represented as a conditioning object that encapsulates the blended text encodings. Type should be `CONDITIONING`.
