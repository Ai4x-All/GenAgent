- `LayerColor_ ColorTemperature`: This node adjusts the color temperature of an image, simulating warmer or cooler lighting conditions. It modifies the image's RGB values based on the specified temperature, enhancing the visual warmth or coolness.
    - Inputs:
        - `image` (Required): The input image to be processed. Adjusting its color temperature simulates different lighting conditions. Type should be `IMAGE`.
        - `temperature` (Required): The temperature value to adjust the image's color temperature. Positive values simulate warmer lighting, while negative values simulate cooler lighting. Type should be `FLOAT`.
    - Outputs:
        - `image`: The image with adjusted color temperature, reflecting the simulated lighting condition. Type should be `IMAGE`.
