- `ImageToImage Settings (JPS)`: The ImageToImage Settings node is designed to configure and apply specific settings for image-to-image transformation tasks within the JPS Nodes framework. It focuses on adjusting parameters that influence how an input image is processed and transformed into an output image, catering to various customization needs for image manipulation.
    - Parameters:
        - `img2img_strength`: Specifies the strength of the image-to-image transformation, affecting the intensity of the applied changes. Type should be `INT`.
        - `inpaint_strength`: Determines the strength of the inpainting effect, influencing how missing or unwanted parts of the image are filled in. Type should be `INT`.
        - `inpaint_grow_mask`: Sets the amount by which the inpainting mask is expanded, affecting the area of the image that is subject to inpainting. Type should be `INT`.
        - `unsampler_strength`: Defines the strength of the unsampling process, affecting the level of detail enhancement in the output image. Type should be `INT`.
        - `unsampler_cfg`: Specifies the configuration for the unsampler, influencing the algorithm's behavior and output quality. Type should be `FLOAT`.
        - `unsampler_sampler`: Selects the sampling method used by the unsampler, affecting the texture and quality of the output image. Type should be `COMBO[STRING]`.
        - `unsampler_scheduler`: Chooses the scheduling algorithm for the unsampling process, impacting the progression and quality of image transformation. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `img2img_settings`: Outputs the configured settings for image-to-image transformation, encapsulating all adjustments made for processing the input image. Type should be `BASIC_PIPE`.