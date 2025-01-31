- `CR Aspect Ratio`: This node is designed to adjust the aspect ratio of images, ensuring they fit specific dimensions or standards. It's particularly useful in scenarios where maintaining the visual integrity of an image across different display sizes or formats is crucial.
    - Inputs:
        - `width` (Required): Specifies the desired width of the output image. This parameter plays a crucial role in determining the final dimensions of the image after aspect ratio adjustments. Type should be `INT`.
        - `height` (Required): Specifies the desired height of the output image. Along with width, this parameter is essential for defining the final dimensions of the image post-adjustment. Type should be `INT`.
        - `aspect_ratio` (Required): Defines the aspect ratio to apply to the image. This parameter is key in ensuring the image fits the desired dimensions while maintaining its visual integrity. Type should be `COMBO[STRING]`.
        - `swap_dimensions` (Required): Determines whether the width and height dimensions should be swapped. This is useful for rotating images or changing their orientation. Type should be `COMBO[STRING]`.
        - `upscale_factor` (Required): Specifies the factor by which the image should be upscaled. This is important for enhancing image quality in larger displays. Type should be `FLOAT`.
        - `prescale_factor` (Required): Specifies the factor by which the image should be prescaled before applying the aspect ratio adjustments. This helps in optimizing the processing for different image sizes. Type should be `FLOAT`.
        - `batch_size` (Required): Defines the number of images to process in a single batch. This parameter is crucial for optimizing performance and resource utilization during batch processing. Type should be `INT`.
    - Outputs:
        - `width`: The adjusted width of the image after applying the aspect ratio adjustments. Type should be `INT`.
        - `height`: The adjusted height of the image after applying the aspect ratio adjustments. Type should be `INT`.
        - `upscale_factor`: The factor by which the image has been upscaled during the aspect ratio adjustment process. Type should be `FLOAT`.
        - `prescale_factor`: The factor by which the image has been prescaled before applying the aspect ratio adjustments. Type should be `FLOAT`.
        - `batch_size`: The number of images processed in the batch. Type should be `INT`.
        - `empty_latent`: A tensor representing the latent space of the processed images. Type should be `LATENT`.
        - `show_help`: A URL to a help page with more information about aspect ratio adjustments. Type should be `STRING`.
