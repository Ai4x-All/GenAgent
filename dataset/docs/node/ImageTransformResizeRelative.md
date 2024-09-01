- `ImageTransformResizeRelative`: The ImageTransformResizeRelative node dynamically resizes images based on relative scale factors for width and height, allowing for flexible image transformations that maintain the aspect ratio or adjust the image size proportionally.
    - Parameters:
        - `scale_width`: Determines the factor by which the width of the images will be scaled, affecting the overall size of the output images. Type should be `FLOAT`.
        - `scale_height`: Determines the factor by which the height of the images will be scaled, affecting the overall size of the output images. Type should be `FLOAT`.
        - `method`: Specifies the interpolation method used for resizing, impacting the quality and characteristics of the resized images. Type should be `COMBO[STRING]`.
    - Inputs:
        - `images`: Specifies the images to be resized, serving as the primary input for the transformation process. Type should be `IMAGE`.
    - Outputs:
        - `image`: Produces resized images according to the specified relative scale factors for width and height. Type should be `IMAGE`.