- `Image Mix RGB Channels`: This node is designed to merge individual red, green, and blue image channels into a single RGB image. It abstracts the complexity of channel manipulation and blending, providing a straightforward way to combine these color components into a cohesive visual representation.
    - Inputs:
        - `red_channel` (Required): The red channel of the image, representing the intensity of the red color component across the image. It plays a crucial role in determining the overall hue and saturation of the merged RGB image. Type should be `IMAGE`.
        - `green_channel` (Required): The green channel of the image, representing the intensity of the green color component. It significantly influences the final color balance and appearance of the merged RGB image. Type should be `IMAGE`.
        - `blue_channel` (Required): The blue channel of the image, indicating the intensity of the blue color component. This channel is essential for achieving the desired depth and tone in the final RGB image. Type should be `IMAGE`.
    - Outputs:
        - `image`: The resulting image after merging the red, green, and blue channels. It is a full-color RGB image that combines the input channels into a single, visually cohesive output. Type should be `IMAGE`.
