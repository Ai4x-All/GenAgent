- `Image Gradient Map`: The node applies a gradient map to an image, optionally flipping the gradient map horizontally. It transforms the input image by mapping its grayscale values to colors defined in the gradient map, creating a visually appealing effect that retains the original image's structure while altering its color scheme.
    - Inputs:
        - `image` (Required): The original image to which the gradient map will be applied. It serves as the base for the transformation, dictating the structure of the output image. Type should be `IMAGE`.
        - `gradient_image` (Required): The gradient map image that defines the color transformation. This image's colors are mapped to the grayscale values of the original image, determining the output image's color scheme. Type should be `IMAGE`.
        - `flip_left_right` (Required): A boolean flag indicating whether the gradient map should be flipped horizontally before being applied. This can alter the visual effect of the gradient mapping on the original image. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The resulting image after applying the gradient map to the original image. This output retains the structure of the original image but features the colors defined by the gradient map. Type should be `IMAGE`.