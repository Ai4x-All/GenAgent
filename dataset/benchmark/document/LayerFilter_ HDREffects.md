- `LayerFilter_ HDREffects`: The HDR Effects node is designed to enhance images by applying High Dynamic Range (HDR) effects, improving contrast, brightness, and color depth to simulate the HDR photography technique. This node aims to make images appear more vivid and closer to what the human eye perceives in real life, by adjusting various parameters such as shadow, highlight, and gamma intensity.
    - Inputs:
        - `image` (Required): The input image to which HDR effects will be applied. This is the primary input for the node, serving as the basis for all subsequent HDR enhancements. Type should be `IMAGE`.
        - `hdr_intensity` (Required): Controls the overall intensity of the HDR effect, affecting how pronounced the HDR enhancements are on the image. Type should be `FLOAT`.
        - `shadow_intensity` (Required): Adjusts the intensity of shadows in the image, making them lighter or darker to enhance depth and detail. Type should be `FLOAT`.
        - `highlight_intensity` (Required): Adjusts the intensity of highlights in the image, enhancing brightness in lighter areas for a more dynamic range. Type should be `FLOAT`.
        - `gamma_intensity` (Required): Controls the gamma correction level, affecting the mid-tones and overall brightness of the image. Type should be `FLOAT`.
        - `contrast` (Required): Adjusts the contrast level of the image, enhancing the difference between light and dark areas. Type should be `FLOAT`.
        - `enhance_color` (Required): Enhances the saturation and vibrancy of colors in the image, making them more vivid and pronounced. Type should be `FLOAT`.
    - Outputs:
        - `image`: The output image after applying HDR effects, showcasing enhanced contrast, brightness, and color depth. Type should be `IMAGE`.