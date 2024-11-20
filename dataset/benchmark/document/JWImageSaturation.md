- `JWImageSaturation`: This node adjusts the saturation level of an input image based on a specified factor, enhancing or reducing the intensity of the image's colors.
    - Inputs:
        - `image` (Required): The input image to adjust the saturation for. The adjustment is made by altering the intensity of the image's colors. Type should be `IMAGE`.
        - `factor` (Required): A multiplier for adjusting the saturation level. A factor greater than 1 increases saturation, making colors more intense, while a factor less than 1 decreases it, making the colors less intense. Type should be `FLOAT`.
    - Outputs:
        - `image`: The output image with adjusted saturation levels. Type should be `IMAGE`.