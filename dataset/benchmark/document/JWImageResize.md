- `JWImageResize`: The JWImageResize node is designed to adjust the size of an image to specified width and height dimensions, using a chosen interpolation method to maintain image quality.
    - Inputs:
        - `image` (Required): The input image tensor to be resized. It's crucial for defining the visual content that will undergo resizing. Type should be `IMAGE`.
        - `height` (Required): Specifies the target height for the resized image, directly influencing the image's vertical dimension. Type should be `INT`.
        - `width` (Required): Determines the target width for the resized image, directly affecting the image's horizontal dimension. Type should be `INT`.
        - `interpolation_mode` (Required): The method used for interpolating between pixel values when resizing, which affects the quality and appearance of the output image. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The resized image tensor, adjusted to the specified dimensions and interpolation quality. Type should be `IMAGE`.