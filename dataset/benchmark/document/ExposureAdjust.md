- `ExposureAdjust`: The ExposureAdjust node is designed to modify the exposure of images by adjusting their brightness levels. It supports different input and output color modes, and optionally applies tonemapping to adjust the dynamic range of the images.
    - Inputs:
        - `images` (Required): The input images to be adjusted for exposure. This parameter is crucial for defining the visual content that will undergo exposure correction. Type should be `IMAGE`.
        - `stops` (Required): Determines the exposure adjustment level. Positive values increase exposure (making the image brighter), while negative values decrease it (making the image darker). Type should be `FLOAT`.
        - `input_mode` (Required): Specifies the color space of the input images, either 'sRGB' or 'linear', affecting how exposure adjustments are applied. Type should be `COMBO[STRING]`.
        - `output_mode` (Required): Defines the color space for the output images, allowing for flexibility in integrating the adjusted images into various workflows. Type should be `COMBO[STRING]`.
        - `use_tonemap` (Required): A boolean flag that indicates whether tonemapping should be applied to the images, useful for handling high dynamic range content. Type should be `BOOLEAN`.
        - `tonemap_scale` (Required): Adjusts the scale of the tonemapping effect, providing control over the dynamic range compression of the images. Type should be `FLOAT`.
    - Outputs:
        - `image`: The output images with adjusted exposure, potentially in a different color space and with optional tonemapping applied. Type should be `IMAGE`.