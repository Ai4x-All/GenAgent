- `KSampler Cycle`: The KSampler Cycle node is designed to perform iterative sampling cycles using a specified sampling strategy. It leverages advanced sampling techniques to generate or modify latent images, incorporating various conditioning and noise parameters to guide the generation process. This node is part of a suite aimed at enhancing image generation capabilities through sophisticated sampling algorithms.
    - Inputs:
        - `model` (Required): Specifies the model to be used for sampling, playing a crucial role in determining the quality and characteristics of the generated images. Type should be `MODEL`.
        - `seed` (Required): The seed parameter ensures reproducibility of the sampling process by initializing the random number generator to a specific state. Type should be `INT`.
        - `steps` (Required): Defines the number of steps to be taken in the sampling process, affecting the detail and quality of the generated images. Type should be `INT`.
        - `cfg` (Required): Controls the conditioning factor in the sampling process, influencing how strongly the positive and negative conditioning affect the generated images. Type should be `FLOAT`.
        - `sampler_name` (Required): Determines the specific sampling algorithm to be used, allowing for customization of the sampling process. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): Specifies the scheduler to manage the sampling steps, enabling fine-tuning of the sampling dynamics. Type should be `COMBO[STRING]`.
        - `positive` (Required): Positive conditioning terms to guide the sampling towards desired attributes or features in the generated images. Type should be `CONDITIONING`.
        - `negative` (Required): Negative conditioning terms to steer the sampling away from certain attributes or features, refining the generation process. Type should be `CONDITIONING`.
        - `latent_image` (Required): The initial latent image to be modified or used as a basis for generation in the sampling cycle. Type should be `LATENT`.
        - `tiled_vae` (Required): Enables or disables the use of tiled VAE, affecting the texture and detail of the generated images. Type should be `COMBO[STRING]`.
        - `latent_upscale` (Required): Specifies the method used for upscaling the latent image, influencing the resolution and quality. Type should be `COMBO[STRING]`.
        - `upscale_factor` (Required): Determines the factor by which the latent image is upscaled, directly impacting its resolution. Type should be `FLOAT`.
        - `upscale_cycles` (Required): Defines the number of cycles for upscaling, affecting the final image quality through iterative refinement. Type should be `INT`.
        - `starting_denoise` (Required): Sets the initial denoise level for the sampling process, influencing the clarity of the generated images from the start. Type should be `FLOAT`.
        - `cycle_denoise` (Required): Adjusts the denoise level for each cycle, allowing for dynamic control over image clarity throughout the sampling process. Type should be `FLOAT`.
        - `scale_denoise` (Required): Enables or disables denoise scaling, affecting the denoise level based on the image scale. Type should be `COMBO[STRING]`.
        - `scale_sampling` (Required): Determines the sampling method used during scaling, impacting the texture and detail of the upscaled image. Type should be `COMBO[STRING]`.
        - `vae` (Required): Specifies the VAE model used in the process, crucial for the generation and manipulation of latent images. Type should be `VAE`.
        - `secondary_model` (Optional): Optional secondary model for enhanced sampling or effects, providing additional customization. Type should be `MODEL`.
        - `secondary_start_cycle` (Optional): Defines the cycle at which the secondary model begins to be applied, allowing for staged sampling processes. Type should be `INT`.
        - `upscale_model` (Optional): Specifies the model used for upscaling, impacting the quality and method of image enlargement. Type should be `UPSCALE_MODEL`.
        - `processor_model` (Optional): Optional processor model for additional image processing or effects during the sampling cycle. Type should be `UPSCALE_MODEL`.
        - `pos_additive` (Optional): Additional positive conditioning terms, enhancing the guidance towards desired features. Type should be `CONDITIONING`.
        - `neg_additive` (Optional): Additional negative conditioning terms, refining the avoidance of certain features. Type should be `CONDITIONING`.
        - `pos_add_mode` (Optional): Determines how the additional positive conditioning is applied, affecting its influence on the generation process. Type should be `COMBO[STRING]`.
        - `pos_add_strength` (Optional): Sets the strength of the additional positive conditioning, controlling its impact on the generated images. Type should be `FLOAT`.
        - `pos_add_strength_scaling` (Optional): Adjusts the scaling of positive conditioning strength, allowing for dynamic influence based on other factors. Type should be `COMBO[STRING]`.
        - `pos_add_strength_cutoff` (Optional): Defines a cutoff for positive conditioning strength, limiting its maximum impact. Type should be `FLOAT`.
        - `neg_add_mode` (Optional): Determines how the additional negative conditioning is applied, affecting its influence on the generation process. Type should be `COMBO[STRING]`.
        - `neg_add_strength` (Optional): Sets the strength of the additional negative conditioning, controlling its impact on the generated images. Type should be `FLOAT`.
        - `neg_add_strength_scaling` (Optional): Adjusts the scaling of negative conditioning strength, allowing for dynamic influence based on other factors. Type should be `COMBO[STRING]`.
        - `neg_add_strength_cutoff` (Optional): Defines a cutoff for negative conditioning strength, limiting its maximum impact. Type should be `FLOAT`.
        - `sharpen_strength` (Optional): Adjusts the strength of image sharpening applied after sampling, affecting image clarity and detail. Type should be `FLOAT`.
        - `sharpen_radius` (Optional): Determines the radius of the sharpening effect, influencing the extent of detail enhancement. Type should be `INT`.
        - `steps_scaling` (Optional): Enables or disables scaling of the number of steps based on certain conditions, affecting the sampling process duration. Type should be `COMBO[STRING]`.
        - `steps_control` (Optional): Specifies the control mechanism for dynamically adjusting the number of sampling steps. Type should be `COMBO[STRING]`.
        - `steps_scaling_value` (Optional): Sets the value for scaling the number of steps, directly impacting the sampling process duration. Type should be `INT`.
        - `steps_cutoff` (Optional): Defines a cutoff for the number of steps, limiting the maximum duration of the sampling process. Type should be `INT`.
        - `denoise_cutoff` (Optional): Sets a cutoff for denoise level, limiting the maximum amount of denoising applied to the generated images. Type should be `FLOAT`.
    - Outputs:
        - `latent(s)`: unknown Type should be `LATENT`.