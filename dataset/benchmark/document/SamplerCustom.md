- `SamplerCustom`: The SamplerCustom node is designed to provide a customizable sampling mechanism within a broader generative modeling or simulation framework. It allows for the dynamic selection and configuration of sampling strategies to adapt to various data distributions or modeling objectives, enhancing the flexibility and efficiency of the generative process.
    - Inputs:
        - `model` (Required): Specifies the generative model to be used for sampling, serving as the core component around which sampling strategies are configured. Type should be `MODEL`.
        - `add_noise` (Required): Determines whether noise should be added to the sampling process, enhancing the diversity of generated samples. Type should be `BOOLEAN`.
        - `noise_seed` (Required): Sets the seed for noise generation, ensuring reproducibility in the sampling process. Type should be `INT`.
        - `cfg` (Required): Controls the conditioning factor, adjusting the influence of specified conditions on the generated samples. Type should be `FLOAT`.
        - `positive` (Required): Defines positive conditioning to guide the sampling towards desired characteristics. Type should be `CONDITIONING`.
        - `negative` (Required): Specifies negative conditioning to steer the sampling away from undesired traits. Type should be `CONDITIONING`.
        - `sampler` (Required): Selects the specific sampling strategy to be employed, allowing for customization of the sampling process. Type should be `SAMPLER`.
        - `sigmas` (Required): Provides control over the noise levels at different stages of the sampling process, enabling fine-tuning of the sample generation. Type should be `SIGMAS`.
        - `latent_image` (Required): Inputs a latent representation of an image to be used as a starting point for the sampling process. Type should be `LATENT`.
    - Outputs:
        - `output`: Outputs the final sampled image in its latent representation, reflecting the applied sampling strategy and conditions. Type should be `LATENT`.
        - `denoised_output`: Provides a denoised version of the sampled image, offering an alternative representation with potentially reduced noise. Type should be `LATENT`.