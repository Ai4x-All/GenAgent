- `ImageResize+`: This node is designed for resizing images to a specified width and height, offering a straightforward way to adjust image dimensions for various applications. It abstracts the complexities of image processing, providing an easy-to-use interface for resizing operations.
    - Inputs:
        - `image` (Required): The input image to be resized. This parameter is crucial as it determines the source image that will undergo the resizing process. Type should be `IMAGE`.
        - `width` (Required): Specifies the desired width of the resized image. This parameter directly influences the output image's dimensions. Type should be `INT`.
        - `height` (Required): Specifies the desired height of the resized image. This parameter directly influences the output image's dimensions. Type should be `INT`.
        - `interpolation` (Required): Defines the method used for interpolating pixels in the resizing process, affecting the quality and appearance of the resized image. Type should be `COMBO[STRING]`.
        - `method` (Required): Determines how the image is resized, influencing whether and how the aspect ratio is preserved or altered. Type should be `COMBO[STRING]`.
        - `condition` (Required): Specifies under what conditions the resizing should occur, allowing for conditional resizing based on the original and target dimensions. Type should be `COMBO[STRING]`.
        - `multiple_of` (Required): Ensures the dimensions of the resized image are multiples of this value, useful for certain processing or model input requirements. Type should be `INT`.
    - Outputs:
        - `IMAGE`: The resized image. This output reflects the changes in dimensions specified by the width and height parameters. Type should be `IMAGE`.
        - `width`: The actual width of the resized image, which may differ from the requested width due to constraints like maintaining aspect ratio or alignment to a multiple. Type should be `INT`.
        - `height`: The actual height of the resized image, which may differ from the requested height due to constraints like maintaining aspect ratio or alignment to a multiple. Type should be `INT`.
