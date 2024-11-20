- `LayerUtility_ ColorImage`: The ColorImage node generates a solid color image based on specified dimensions and color. It serves as a utility for creating background layers or color fills in image processing workflows.
    - Inputs:
        - `width` (Required): Specifies the width of the generated image. It determines how wide the image will be. Type should be `INT`.
        - `height` (Required): Specifies the height of the generated image. It determines the height of the image. Type should be `INT`.
        - `color` (Required): Defines the color of the generated image. The color is specified in a string format, typically as a hex code. Type should be `STRING`.
    - Outputs:
        - `image`: The output is a solid color image with the specified dimensions and color. Type should be `IMAGE`.