- `Automatic CFG - Advanced`: This node represents an advanced configuration for dynamic control flow graph (CFG) adjustments in models, aiming to enhance model performance and flexibility by applying sophisticated CFG modifications.
    - Parameters:
        - `automatic_cfg`: Specifies the level of automatic CFG adjustments to be applied, ranging from basic to advanced configurations. Type should be `COMBO[STRING]`.
        - `skip_uncond`: Determines whether unconditional generation steps should be skipped, optimizing the model's performance for specific tasks. Type should be `BOOLEAN`.
        - `uncond_sigma_start`: The starting sigma value for unconditional generation, part of the fine-tuning parameters for model optimization. Type should be `FLOAT`.
        - `uncond_sigma_end`: The ending sigma value for unconditional generation, concluding the fine-tuning process for model optimization. Type should be `FLOAT`.
        - `lerp_uncond`: Indicates whether linear interpolation is used for unconditional generation, enhancing the model's adaptability. Type should be `BOOLEAN`.
        - `lerp_uncond_strength`: The strength of linear interpolation for unconditional generation, adjusting the intensity of the effect. Type should be `FLOAT`.
        - `lerp_uncond_sigma_start`: The starting sigma value for linear interpolation in unconditional generation, setting the initial condition for the interpolation. Type should be `FLOAT`.
        - `lerp_uncond_sigma_end`: The ending sigma value for linear interpolation in unconditional generation, finalizing the interpolation conditions. Type should be `FLOAT`.
        - `subtract_latent_mean`: Determines whether the mean of the latent space should be subtracted, affecting the model's generation process. Type should be `BOOLEAN`.
        - `subtract_latent_mean_sigma_start`: The starting sigma value for subtracting the latent mean, influencing the adjustment's initiation. Type should be `FLOAT`.
        - `subtract_latent_mean_sigma_end`: The ending sigma value for subtracting the latent mean, marking the adjustment's conclusion. Type should be `FLOAT`.
        - `latent_intensity_rescale`: Indicates whether the intensity of the latent space should be rescaled, modifying the model's output. Type should be `BOOLEAN`.
        - `latent_intensity_rescale_method`: Specifies the method used for rescaling the intensity of the latent space, impacting the model's behavior. Type should be `COMBO[STRING]`.
        - `latent_intensity_rescale_cfg`: The configuration value for rescaling the latent intensity, determining the scale of adjustment. Type should be `FLOAT`.
        - `latent_intensity_rescale_sigma_start`: The starting sigma value for rescaling the latent intensity, setting the initial parameters for the rescale. Type should be `FLOAT`.
        - `latent_intensity_rescale_sigma_end`: The ending sigma value for rescaling the latent intensity, finalizing the parameters for the adjustment. Type should be `FLOAT`.
    - Inputs:
        - `model`: The model to which the advanced dynamic CFG adjustments will be applied, serving as the foundation for the enhancements. Type should be `MODEL`.
    - Outputs:
        - `model`: The enhanced model with advanced dynamic CFG adjustments applied, ready for improved performance and flexibility. Type should be `MODEL`.