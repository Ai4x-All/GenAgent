- `Unary Image Op`: This node applies a specified unary operation on an image, such as inversion, averaging, rounding, clamping, or taking the absolute value. It's designed to manipulate the pixel values of an image according to the chosen operation, enabling various image preprocessing tasks.
    - Inputs:
        - `image` (Required): The image to be processed. It serves as the primary input for the operation, determining the visual content that will undergo the specified unary transformation. Type should be `IMAGE`.
        - `op` (Required): Specifies the unary operation to apply to the image. Options include 'invert', 'average', 'round', 'clamp', and 'abs', each affecting the image's pixel values in a unique way. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The processed image, after applying the specified unary operation. It reflects the visual changes made to the original image based on the operation performed. Type should be `IMAGE`.
