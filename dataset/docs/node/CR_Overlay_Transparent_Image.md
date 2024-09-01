- `CR Overlay Transparent Image`: This node is designed to overlay a transparent image onto a background image, allowing for adjustments in transparency, position, rotation, and scale of the overlay image. It facilitates the creation of composite images by blending two images together in a visually appealing manner.
    - Parameters:
        - `transparency`: Controls the opacity of the overlay image, allowing it to be more or less visible against the background image. Type should be `FLOAT`.
        - `offset_x`: The horizontal offset from the center of the background image where the overlay image will be placed. Type should be `INT`.
        - `offset_y`: The vertical offset from the center of the background image where the overlay image will be placed. Type should be `INT`.
        - `rotation_angle`: The angle in degrees to rotate the overlay image, enabling dynamic positioning and orientation. Type should be `FLOAT`.
        - `overlay_scale_factor`: A factor by which the overlay image is scaled, allowing for adjustments in size relative to the background image. Type should be `FLOAT`.
    - Inputs:
        - `back_image`: The background image onto which the overlay image will be placed. It serves as the base layer for the composite image. Type should be `IMAGE`.
        - `overlay_image`: The image to be overlaid on the background image. This image can be manipulated in terms of transparency, rotation, and scale to achieve the desired visual effect. Type should be `IMAGE`.
    - Outputs:
        - `image`: The resulting image after overlaying the transparent image onto the background, incorporating all specified transformations. Type should be `IMAGE`.