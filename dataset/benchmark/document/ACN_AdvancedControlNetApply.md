- `ACN_AdvancedControlNetApply`: This node applies advanced control net transformations to conditioning data, enhancing image generation with more nuanced control and customization options. It leverages advanced features of control nets to modify and fine-tune the conditioning process, allowing for sophisticated manipulation of image attributes.
    - Inputs:
        - `positive` (Required): Positive conditioning data that will be enhanced through the application of control net transformations, contributing to the generation of desired image attributes. Type should be `CONDITIONING`.
        - `negative` (Required): Negative conditioning data that will be modified by control net transformations to avoid certain image attributes, ensuring the generated image aligns with specified preferences. Type should be `CONDITIONING`.
        - `control_net` (Required): The advanced control net model used to apply transformations to the conditioning data, enabling the customization and fine-tuning of image attributes. Type should be `CONTROL_NET`.
        - `image` (Required): The input image to which the control net transformations are applied, serving as a canvas for the enhanced conditioning effects. Type should be `IMAGE`.
        - `strength` (Required): A scalar value determining the intensity of the control net transformations applied to the conditioning data, allowing for fine-tuning of the effect's strength. Type should be `FLOAT`.
        - `start_percent` (Required): Defines the starting percentage of the effect's application, allowing for gradual introduction of the control net transformations over the image. Type should be `FLOAT`.
        - `end_percent` (Required): Specifies the ending percentage for the application of control net transformations, enabling a controlled and gradual effect on the image. Type should be `FLOAT`.
        - `mask_optional` (Optional): An optional mask that can be applied to selectively target areas for control net transformations, enhancing precision in image manipulation. Type should be `MASK`.
        - `timestep_kf` (Optional): Optional keyframe for timestep control, allowing for dynamic adjustment of transformation application over time. Type should be `TIMESTEP_KEYFRAME`.
        - `latent_kf_override` (Optional): Optional override for latent keyframes, providing advanced control over the conditioning process through specific latent manipulations. Type should be `LATENT_KEYFRAME`.
        - `weights_override` (Optional): Optional weights override for the control net, offering further customization of the transformation effects based on specific weight adjustments. Type should be `CONTROL_NET_WEIGHTS`.
        - `model_optional` (Optional): An optional model parameter that can be used in conjunction with the control net for enhanced conditioning effects. Type should be `MODEL`.
        - `vae_optional` (Optional): An optional VAE parameter that can be utilized for additional conditioning manipulations, enriching the image generation process. Type should be `VAE`.
        - `autosize` (Optional): Optional autosizing parameter that automatically adjusts the image size for optimal processing, enhancing the efficiency of transformation application. Type should be `ACNAUTOSIZE`.
    - Outputs:
        - `positive`: The enhanced positive conditioning data after the application of advanced control net transformations. Type should be `CONDITIONING`.
        - `negative`: The modified negative conditioning data following the application of control net transformations, tailored to avoid specific attributes. Type should be `CONDITIONING`.
        - `model_opt`: An optional output model that has been adjusted through the control net application process, reflecting changes in conditioning effects. Type should be `MODEL`.
