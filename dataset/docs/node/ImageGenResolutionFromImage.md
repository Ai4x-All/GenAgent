- `ImageGenResolutionFromImage`: This node is designed to compute the generation resolution from an input image. It analyzes the dimensions of the provided image and calculates the width and height that should be used for image generation, ensuring the output resolution is directly derived from the input image's size.
    - Parameters:
    - Inputs:
        - `image`: The input image for which the generation resolution is to be calculated. This parameter is crucial as it directly influences the output resolution by analyzing the image's dimensions. Type should be `IMAGE`.
    - Outputs:
        - `IMAGE_GEN_WIDTH (INT)`: The calculated width for image generation, derived from the input image's dimensions. Type should be `INT`.
        - `IMAGE_GEN_HEIGHT (INT)`: The calculated height for image generation, derived from the input image's dimensions. Type should be `INT`.