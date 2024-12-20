- `ImageAlphaComposite`: The ImageAlphaComposite node is designed for blending two images together based on their alpha values to create a single composited image. This process involves combining the visual elements of both input images into one, taking into account transparency and layering effects.
    - Inputs:
        - `image_i` (Required): The second image to be composited. It acts as the other base layer in the alpha compositing process, layered together with the first image. Type should be `IMAGE`.
    - Outputs:
        - `image`: The resulting image after alpha compositing, blending the input images based on their alpha values. Type should be `IMAGE`.
