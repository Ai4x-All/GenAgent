- `UltimateSDUpscaleCustomSample`: This node specializes in enhancing image quality through upscaling, leveraging advanced techniques to refine image details and textures. It extends the capabilities of standard upscaling by allowing for custom model and sampling parameters, providing a tailored approach to image enhancement.
    - Inputs:
        - `image` (Required): The original image to be upscaled. This is the starting point for the upscaling process. Type should be `IMAGE`.
        - `model` (Required): The generative model used for enhancing the image, which plays a crucial role in the upscaling process. Type should be `MODEL`.
        - `positive` (Required): Positive conditioning text to guide the model in enhancing specific aspects of the image. Type should be `CONDITIONING`.
        - `negative` (Required): Negative conditioning text to instruct the model on what aspects to avoid or minimize in the image. Type should be `CONDITIONING`.
        - `vae` (Required): The variational autoencoder used in conjunction with the model to improve the upscaling results. Type should be `VAE`.
        - `upscale_by` (Required): The factor by which the image will be upscaled, determining the increase in resolution. Type should be `FLOAT`.
        - `seed` (Required): A seed value for random number generation, ensuring reproducibility of the upscaling process. Type should be `INT`.
        - `steps` (Required): The number of steps the model will take in enhancing the image, affecting the detail and quality of the output. Type should be `INT`.
        - `cfg` (Required): The classifier-free guidance scale, adjusting the influence of the conditioning texts on the upscaling process. Type should be `FLOAT`.
        - `sampler_name` (Required): The name of the sampler used in the upscaling process, affecting the texture and details of the upscaled image. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): The scheduler for the sampling process, managing how the model iterates over the image. Type should be `COMBO[STRING]`.
        - `denoise` (Required): The amount of denoising applied during upscaling, affecting the smoothness and clarity of the image. Type should be `FLOAT`.
        - `mode_type` (Required): The mode of operation for upscaling, which can include different strategies for handling image tiles and seams. Type should be `COMBO[STRING]`.
        - `tile_width` (Required): The width of the tiles used in the upscaling process, which can affect the performance and quality of the output. Type should be `INT`.
        - `tile_height` (Required): The height of the tiles used in the upscaling process, similar to tile width in its impact on the upscaling. Type should be `INT`.
        - `mask_blur` (Required): The level of blur applied to the mask used in tiled upscaling, affecting the blending of tiles. Type should be `INT`.
        - `tile_padding` (Required): The padding added around each tile during upscaling, which helps in reducing visible seams between tiles. Type should be `INT`.
        - `seam_fix_mode` (Required): The method used for fixing seams between tiles, crucial for achieving a seamless upscale. Type should be `COMBO[STRING]`.
        - `seam_fix_denoise` (Required): The amount of denoising applied specifically to the seams, improving the overall smoothness of the image. Type should be `FLOAT`.
        - `seam_fix_width` (Required): The width of the area around seams to be fixed, affecting the transition between tiles. Type should be `INT`.
        - `seam_fix_mask_blur` (Required): The level of blur applied to the seam fix mask, affecting how seamlessly the fixed seams blend with the rest of the image. Type should be `INT`.
        - `seam_fix_padding` (Required): The padding around the seam fix area, used to further blend and smooth out the transitions between tiles. Type should be `INT`.
        - `force_uniform_tiles` (Required): A flag indicating whether to use uniform tile sizes throughout the image, which can affect the consistency of the upscale. Type should be `BOOLEAN`.
        - `tiled_decode` (Required): Indicates whether the decoding process should be done in a tiled manner, affecting the handling of large images. Type should be `BOOLEAN`.
        - `upscale_model` (Optional): Specifies the model used for upscaling, enabling the selection of different algorithms or models tailored to specific upscaling needs. Type should be `UPSCALE_MODEL`.
        - `custom_sampler` (Optional): Defines a custom sampling method for the upscaling process, allowing for more control over the sampling techniques used during image enhancement. Type should be `SAMPLER`.
        - `custom_sigmas` (Optional): Allows for the customization of sigma values used in the sampling process, offering fine-tuning of the noise levels applied during image upscaling. Type should be `SIGMAS`.
    - Outputs:
        - `image`: The output is an enhanced version of the input image, with improved resolution and detail quality through the upscaling process. Type should be `IMAGE`.