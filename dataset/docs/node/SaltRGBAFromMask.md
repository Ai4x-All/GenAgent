- `SaltRGBAFromMask`: This node is designed to convert masks into RGBA images, incorporating transparency into the resulting image. It focuses on processing image masks to generate images with an alpha channel, enabling the creation of images where certain regions are transparent, based on the input mask.
    - Parameters:
        - `threshold`: A value used to determine the cutoff point for what is considered transparent in the mask. Pixels in the mask above this value will be more opaque. Type should be `FLOAT`.
        - `invert_mask`: A boolean indicating whether the mask should be inverted before applying it to the image. Inverting the mask swaps which areas are considered transparent and which are opaque. Type should be `BOOLEAN`.
    - Inputs:
        - `image`: The source image that will be combined with the mask to produce an RGBA image. The image's non-masked areas will remain visible, while the masked areas can be made transparent or semi-transparent. Type should be `IMAGE`.
        - `mask`: The input mask for which the RGBA image will be generated. This mask determines the regions that will be transparent or opaque in the resulting image. Type should be `MASK`.
    - Outputs:
        - `rgba_image`: The resulting RGBA image where the input mask has been applied to define transparent regions. Type should be `IMAGE`.