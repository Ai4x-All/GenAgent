- `LDSRUpscaler`: The LDSRUpscaler node is designed to upscale images using the LDSR model, providing a high-level interface for enhancing image resolution through deep learning techniques. It abstracts the complexities of the underlying LDSR model operations, offering a simplified method for users to improve image quality with options for pre and post downscaling and different downsample methods.
    - Parameters:
        - `model`: Specifies the LDSR model to be used for upscaling. This model determines the upscaling technique and quality. Type should be `COMBO[STRING]`.
        - `steps`: Defines the number of steps for the upscaling process, affecting the quality and computation time of the upscaling. Type should be `COMBO[STRING]`.
        - `pre_downscale`: Optional pre-processing step to downscale images before upscaling, which can affect the final image quality and processing time. Type should be `COMBO[STRING]`.
        - `post_downscale`: Optional post-processing step to adjust the size of the upscaled images, allowing for customization of the output resolution. Type should be `COMBO[STRING]`.
        - `downsample_method`: The method used for downsampling during the pre and post downscale steps, influencing the quality of the downscaled images. Type should be `COMBO[STRING]`.
    - Inputs:
        - `images`: The images to be upscaled. This input allows for batch processing of multiple images, enhancing their resolution. Type should be `IMAGE`.
    - Outputs:
        - `images`: The upscaled images, enhanced in resolution through the LDSR upscaling process. Type should be `IMAGE`.