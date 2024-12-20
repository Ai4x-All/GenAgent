- `Prepare Image (JPS)`: The Prepare Image node is designed to process and adjust images according to specified parameters such as resizing, cropping, padding, and applying various transformations like interpolation and sharpening. This node aims to prepare images for further processing or analysis, ensuring they meet the required dimensions and quality standards.
    - Inputs:
        - `image` (Required): The input image to be processed. This parameter is crucial as it serves as the base for all subsequent adjustments and transformations. Type should be `IMAGE`.
        - `target_w` (Required): The target width for the image after processing. It determines the final width that the image will be resized or adjusted to. Type should be `INT`.
        - `target_h` (Required): The target height for the image after processing. It determines the final height that the image will be resized or adjusted to. Type should be `INT`.
        - `crop_w_percent` (Required): The percentage of the image's width to be retained after cropping. This parameter allows for precise control over the width of the cropped area. Type should be `INT`.
        - `crop_h_percent` (Required): The percentage of the image's height to be retained after cropping. This parameter allows for precise control over the height of the cropped area. Type should be `INT`.
        - `offset_w` (Required): The horizontal offset applied to the image. This parameter can be used to shift the image horizontally before other transformations are applied. Type should be `INT`.
        - `offset_h` (Required): The vertical offset applied to the image. This parameter can be used to shift the image vertically before other transformations are applied. Type should be `INT`.
        - `interpolation` (Required): The interpolation method to be used during image resizing. This parameter affects the quality of the resized image. Type should be `COMBO[STRING]`.
        - `sharpening` (Required): The level of sharpening to apply to the image. This parameter enhances the image's details and clarity. Type should be `FLOAT`.
    - Outputs:
        - `IMAGE`: The processed image after applying the specified adjustments and transformations. Type should be `IMAGE`.
