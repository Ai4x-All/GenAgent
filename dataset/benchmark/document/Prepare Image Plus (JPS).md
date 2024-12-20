- `Prepare Image Plus (JPS)`: The Prepare Image Plus node is designed to configure and apply a set of image preparation settings, including resizing, cropping, padding, interpolation, sharpening, and flipping. It allows for detailed customization of how an image is processed before being used in further operations, ensuring that images are optimally prepared for tasks such as machine learning model input or visual presentation.
    - Inputs:
        - `image` (Required): The primary image input for processing. This parameter is essential as it specifies the image to which all preparation settings will be applied. Type should be `IMAGE`.
        - `target_w` (Required): Specifies the target width for the image after resizing, affecting the final dimensions of the processed image. Type should be `INT`.
        - `target_h` (Required): Specifies the target height for the image after resizing, impacting the final dimensions of the processed image. Type should be `INT`.
        - `offset_w` (Required): Determines the horizontal offset applied to the image, which can adjust the image's position or alignment. Type should be `INT`.
        - `offset_h` (Required): Determines the vertical offset applied to the image, impacting the image's position or alignment vertically. Type should be `INT`.
        - `crop_left` (Required): Specifies the amount of cropping from the left side of the image, useful for removing unwanted edges or framing the subject. Type should be `INT`.
        - `crop_right` (Required): Specifies the amount of cropping from the right side of the image, aiding in framing the subject or removing extraneous parts. Type should be `INT`.
        - `crop_top` (Required): Determines the amount of cropping from the top of the image, which can help in adjusting the framing or focusing on specific parts of the image. Type should be `INT`.
        - `crop_bottom` (Required): Determines the amount of cropping from the bottom of the image, useful for framing or removing unnecessary parts. Type should be `INT`.
        - `padding_left` (Required): Specifies the amount of padding added to the left side of the image, which can be used for alignment or aesthetic purposes. Type should be `INT`.
        - `padding_right` (Required): Specifies the amount of padding added to the right side of the image, aiding in alignment or visual design. Type should be `INT`.
        - `padding_top` (Required): Determines the amount of padding added to the top of the image, which can be used for alignment or to achieve a specific visual effect. Type should be `INT`.
        - `padding_bottom` (Required): Determines the amount of padding added to the bottom of the image, useful for alignment or achieving a desired visual layout. Type should be `INT`.
        - `interpolation` (Required): Defines the method used for resizing the image, impacting the quality and appearance of the resized image. Type should be `COMBO[STRING]`.
        - `sharpening` (Required): Specifies the level of sharpening applied to the image, enhancing edge definition and detail. Type should be `FLOAT`.
        - `resize_type` (Required): Determines the method of resizing applied to the image, such as stretching or cropping to fit the specified dimensions. Type should be `COMBO[STRING]`.
        - `flip` (Required): Indicates whether the image should be flipped horizontally, vertically, or not at all, affecting the image's orientation. Type should be `COMBO[STRING]`.
    - Outputs:
        - `IMAGE`: The output is the image after applying the specified preparation settings, including resizing, cropping, padding, interpolation, sharpening, and flipping. Type should be `IMAGE`.
