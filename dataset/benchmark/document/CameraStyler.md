- `CameraStyler`: The CameraStyler node is designed to apply specific stylistic adjustments to images based on camera settings, such as elevation and azimuth. It utilizes camera embeddings to influence the style transformation, aiming to enhance the visual appeal or realism of the image according to the simulated camera parameters.
    - Inputs:
        - `text_positive` (Required): unknown Type should be `STRING`.
        - `text_negative` (Required): unknown Type should be `STRING`.
        - `camera` (Required): unknown Type should be `COMBO[STRING]`.
        - `log_prompt` (Required): unknown Type should be `BOOLEAN`.
    - Outputs:
        - `text_positive`: unknown Type should be `STRING`.
        - `text_negative`: unknown Type should be `STRING`.
