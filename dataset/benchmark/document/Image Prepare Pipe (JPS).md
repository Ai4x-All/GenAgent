- `Image Prepare Pipe (JPS)`: The Image Prepare Pipe node is designed to configure and apply various preprocessing steps to images before they are processed further. This includes setting parameters for resizing, cropping, padding, interpolation, and sharpening to prepare images for optimal processing in subsequent stages.
    - Inputs:
        - `imageprepare_settings` (Required): Specifies the settings for image preparation, including resizing, cropping, padding, interpolation, and sharpening. This configuration is crucial for tailoring the image processing pipeline to the specific needs of the application. Type should be `BASIC_PIPE`.
    - Outputs:
        - `offset_width`: The horizontal offset applied to the image during preparation. Type should be `INT`.
        - `offset_height`: The vertical offset applied to the image during preparation. Type should be `INT`.
        - `crop_left`: The amount of cropping from the left side of the image. Type should be `INT`.
        - `crop_right`: The amount of cropping from the right side of the image. Type should be `INT`.
        - `crop_top`: The amount of cropping from the top of the image. Type should be `INT`.
        - `crop_bottom`: The amount of cropping from the bottom of the image. Type should be `INT`.
        - `padding_left`: The amount of padding added to the left side of the image. Type should be `INT`.
        - `padding_right`: The amount of padding added to the right side of the image. Type should be `INT`.
        - `padding_top`: The amount of padding added to the top of the image. Type should be `INT`.
        - `padding_bottom`: The amount of padding added to the bottom of the image. Type should be `INT`.
        - `interpolation`: The interpolation method used during image resizing. Type should be `COMBO[STRING]`.
        - `sharpening`: The level of sharpening applied to the image. Type should be `FLOAT`.