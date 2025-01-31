- `EmptyImage`: The EmptyImage node is designed to generate blank images of specified dimensions and color. It allows for the creation of uniform color images that can serve as backgrounds or placeholders in various image processing tasks.
    - Inputs:
        - `width` (Required): Specifies the width of the generated image. It determines how wide the image will be. Type should be `INT`.
        - `height` (Required): Determines the height of the generated image. It affects the vertical size of the image. Type should be `INT`.
        - `batch_size` (Required): Indicates the number of images to generate in a single batch. This allows for the creation of multiple images at once. Type should be `INT`.
        - `color` (Required): Defines the color of the generated image using a hexadecimal value, allowing for customization of the image's appearance. This parameter enables the selection of a wide range of colors. Type should be `INT`.
    - Outputs:
        - `image`: The output is a tensor representing the generated image or images, with the specified dimensions and color. Type should be `IMAGE`.
