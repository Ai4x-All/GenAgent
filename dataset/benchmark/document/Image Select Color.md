- `Image Select Color`: This node is designed to filter and highlight pixels within a specified color range in an image. It allows users to select a color by specifying RGB values and a variance, then creates a new image highlighting only those pixels that fall within the defined color range. This functionality is useful for tasks such as color-based segmentation or identifying objects of a specific color within an image.
    - Inputs:
        - `image` (Required): The input image to be processed. The node will highlight pixels within the specified color range of this image. Type should be `IMAGE`.
        - `red` (Required): The red component of the target color. This value, along with the specified variance, defines the range of red values to be highlighted in the image. Type should be `INT`.
        - `green` (Required): The green component of the target color. This value, along with the specified variance, defines the range of green values to be highlighted in the image. Type should be `INT`.
        - `blue` (Required): The blue component of the target color. This value, along with the specified variance, defines the range of blue values to be highlighted in the image. Type should be `INT`.
        - `variance` (Required): The allowed variance from the specified RGB values. This defines the tolerance for what is considered a match to the target color, allowing for slight variations. Type should be `INT`.
    - Outputs:
        - `image`: The output image where only pixels within the specified color range are highlighted. Pixels outside this range are set to black, focusing attention on the selected color. Type should be `IMAGE`.