- `ColorBlend`: The ColorBlend node is designed to blend two images, specifically a black and white layer with a color layer, to produce a single image that combines the luminosity of the black and white layer with the color information of the color layer. This blending process is achieved through a sophisticated manipulation of color spaces and image processing techniques.
    - Inputs:
        - `bw_layer` (Required): The black and white layer image to be blended. It serves as the base for the luminosity channel in the blending process, influencing the final image's light and dark areas. Type should be `IMAGE`.
        - `color_layer` (Required): The color layer image to be blended. This layer provides the color information for the blending process, affecting the final image's coloration and vibrancy. Type should be `IMAGE`.
    - Outputs:
        - `image`: The result of blending the black and white layer with the color layer, producing an image that combines the luminosity of the former with the color information of the latter. Type should be `IMAGE`.