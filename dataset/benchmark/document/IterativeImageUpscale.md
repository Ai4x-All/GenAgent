- `IterativeImageUpscale`: The IterativeImageUpscale node is designed to enhance the resolution of images through a process that iteratively applies image upscaling techniques. This node aims to improve image quality and detail, making it suitable for applications requiring high-resolution images from lower-resolution sources.
    - Inputs:
        - `pixels` (Required): The 'pixels' parameter represents the input image data in pixel format, serving as the foundation for the upscaling process. Type should be `IMAGE`.
        - `upscale_factor` (Required): The 'upscale_factor' parameter specifies the multiplier for increasing the resolution of the image, directly impacting the upscaling intensity. Type should be `FLOAT`.
        - `steps` (Required): The 'steps' parameter determines the number of iterations or steps the upscaling process will undergo, affecting the gradual improvement in image quality. Type should be `INT`.
        - `temp_prefix` (Required): The 'temp_prefix' parameter is used for specifying a temporary file prefix for intermediate results, aiding in debugging or intermediate analysis. Type should be `STRING`.
        - `upscaler` (Required): The 'upscaler' parameter indicates the upscaling model or technique to be used, influencing the method of resolution enhancement. Type should be `UPSCALER`.
        - `vae` (Required): The 'vae' parameter refers to the variational autoencoder used in the process, crucial for encoding and decoding images during upscaling. Type should be `VAE`.
        - `step_mode` (Required): The 'step_mode' parameter defines the mode of operation for each upscaling step, such as 'simple' or other advanced methods, affecting the approach to image enhancement. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The output is a higher-resolution version of the input image, achieved through iterative upscaling techniques. Type should be `IMAGE`.
