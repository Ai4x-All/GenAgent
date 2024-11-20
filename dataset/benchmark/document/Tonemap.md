- `Tonemap`: The Tonemap node is designed to adjust the tonal range of images to make them suitable for display on different devices or for achieving specific visual effects. It supports conversion between linear and sRGB color spaces and allows for scaling of the tonemap effect.
    - Inputs:
        - `images` (Required): The input images to be tonemapped. This is the primary data the node operates on, affecting the visual outcome based on the tonemap process. Type should be `IMAGE`.
        - `input_mode` (Required): Specifies the color space of the input images, either linear or sRGB, determining the initial conversion step before tonemapping. Type should be `COMBO[STRING]`.
        - `output_mode` (Required): Defines the color space for the output images, choosing between linear and sRGB, to ensure the images are in the desired format after tonemapping. Type should be `COMBO[STRING]`.
        - `tonemap_scale` (Required): A scale factor that adjusts the intensity of the tonemap effect, allowing for finer control over the visual appearance of the output images. Type should be `FLOAT`.
    - Outputs:
        - `image`: The output images after applying the tonemap process, adjusted for tonal range and color space as specified by the input parameters. Type should be `IMAGE`.