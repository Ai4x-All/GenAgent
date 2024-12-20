- `Image Remove Background Rembg (mtb)`: This node specializes in removing the background from images using the Rembg tool, enhancing the focus on the primary subject by isolating it from its surroundings.
    - Inputs:
        - `image` (Required): The input image from which the background is to be removed. It is the primary data on which the background removal process is executed. Type should be `IMAGE`.
        - `alpha_matting` (Required): A boolean flag indicating whether alpha matting is to be applied for finer edge handling in the background removal process. Type should be `BOOLEAN`.
        - `alpha_matting_foreground_threshold` (Required): Defines the threshold for foreground selection in the alpha matting process, affecting the precision of the subject's edges. Type should be `INT`.
        - `alpha_matting_background_threshold` (Required): Sets the threshold for background selection in the alpha matting process, influencing the accuracy of background removal. Type should be `INT`.
        - `alpha_matting_erode_size` (Required): Determines the erode size in the alpha matting process, impacting the smoothness of the subject's edges. Type should be `INT`.
        - `post_process_mask` (Required): A boolean flag that enables post-processing of the mask to refine the background removal results. Type should be `BOOLEAN`.
        - `bgcolor` (Required): Specifies the background color to be applied post-removal, allowing for customization of the resulting image's backdrop. Type should be `COLOR`.
    - Outputs:
        - `Image (rgba)`: The resulting image with the background removed, presented in RGBA format to include transparency information. Type should be `IMAGE`.
        - `Mask`: The mask generated during the background removal process, indicating areas of foreground and background. Type should be `MASK`.
        - `Image`: The final image after background removal, without the alpha channel, suitable for use in contexts where transparency is not required. Type should be `IMAGE`.
