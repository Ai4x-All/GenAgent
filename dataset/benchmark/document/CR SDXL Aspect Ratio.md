- `CR SDXL Aspect Ratio`: This node is designed to adjust the aspect ratio of images specifically for the SDXL model, accommodating a variety of predefined aspect ratios to fit different use cases, such as portraits, landscapes, and cinema formats. It allows for customization of image dimensions based on the selected aspect ratio, ensuring that the output images are optimally sized for the SDXL model's requirements.
    - Inputs:
        - `width` (Required): Specifies the initial width of the image before aspect ratio adjustment. It serves as a base dimension that might be altered based on the selected aspect ratio. Type should be `INT`.
        - `height` (Required): Specifies the initial height of the image before aspect ratio adjustment. It acts as a base dimension that might be modified according to the chosen aspect ratio. Type should be `INT`.
        - `aspect_ratio` (Required): Determines the target aspect ratio for the image, offering a selection of predefined ratios tailored for the SDXL model. This choice dictates the final dimensions of the output image. Type should be `COMBO[STRING]`.
        - `swap_dimensions` (Required): Allows for the swapping of width and height dimensions of the image, accommodating orientation adjustments as needed. Type should be `COMBO[STRING]`.
        - `upscale_factor` (Required): Defines the factor by which the image's dimensions are scaled up, enhancing the resolution of the output image. Type should be `FLOAT`.
        - `batch_size` (Required): Specifies the number of images to process in a single batch, facilitating efficient batch processing of images. Type should be `INT`.
    - Outputs:
        - `width`: The adjusted width of the image after applying the selected aspect ratio and any scaling. Type should be `INT`.
        - `height`: The adjusted height of the image after applying the selected aspect ratio and any scaling. Type should be `INT`.
        - `upscale_factor`: The factor by which the image's dimensions have been scaled up. Type should be `FLOAT`.
        - `batch_size`: The number of images processed in the batch. Type should be `INT`.
        - `empty_latent`: unknown Type should be `LATENT`.
        - `show_help`: A URL to a help page providing additional information and guidance on using the aspect ratio node. Type should be `STRING`.
