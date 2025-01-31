- `KSamplerSeq2`: KSamplerSeq2 is designed for advanced sequence-based sampling in generative models, allowing for complex conditioning, noise manipulation, and latent space operations. It supports iterative sampling with customizable denoising, latent interpolation, and conditioning strategies to generate high-quality samples.
    - Inputs:
        - `model` (Required): Specifies the generative model to be used for sampling. It is crucial for defining the architecture and parameters that will generate the output. Type should be `MODEL`.
        - `seed` (Required): Determines the initial random seed for sampling, enabling reproducibility and variation in the generated sequences. Type should be `INT`.
        - `seed_mode_seq` (Required): Controls how the seed value changes across sequence iterations, affecting the diversity and coherence of the generated samples. Type should be `COMBO[STRING]`.
        - `alternate_values` (Required): Enables or disables the alternation of certain parameters between sequence iterations, introducing variability in the sampling process. Type should be `BOOLEAN`.
        - `steps` (Required): Defines the number of steps to be taken in the sampling process, impacting the detail and quality of the generated samples. Type should be `INT`.
        - `cfg` (Required): Sets the configuration for the sampling process, influencing the balance between fidelity to the input conditions and creativity. Type should be `FLOAT`.
        - `sampler_name` (Required): Selects the specific sampling algorithm to be used, affecting the characteristics of the generated samples. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): Chooses the scheduling algorithm for controlling the sampling process, impacting the progression and quality of samples. Type should be `COMBO[STRING]`.
        - `frame_count` (Required): Specifies the total number of frames to be generated in the sequence, affecting the overall length and complexity of the output. Type should be `INT`.
        - `cond_keyframes` (Required): Determines the number of keyframes for conditioning, influencing the variation and transitions in the generated sequence. Type should be `INT`.
        - `positive_seq` (Required): Specifies the positive conditioning sequence for the sampling, guiding the generative model towards desired attributes. Type should be `CONDITIONING`.
        - `negative_seq` (Required): Specifies the negative conditioning sequence for the sampling, steering the generative model away from undesired attributes. Type should be `CONDITIONING`.
        - `use_conditioning_slerp` (Required): Enables spherical linear interpolation for conditioning, allowing for smooth transitions between conditions in the sequence. Type should be `BOOLEAN`.
        - `cond_slerp_strength` (Required): Controls the strength of the conditioning spherical linear interpolation, affecting the smoothness of condition transitions. Type should be `FLOAT`.
        - `latent_image` (Required): Provides the initial latent image for the sampling process, serving as the starting point for generation. Type should be `LATENT`.
        - `use_latent_interpolation` (Required): Enables latent space interpolation between steps, introducing smooth transitions and variations in the generated sequence. Type should be `BOOLEAN`.
        - `latent_interpolation_mode` (Required): Determines the method of latent space interpolation, affecting the nature of transitions between generated samples. Type should be `COMBO[STRING]`.
        - `latent_interp_strength` (Required): Controls the strength of latent space interpolation, influencing the degree of variation between sequence steps. Type should be `FLOAT`.
        - `denoise_start` (Required): Sets the initial denoising level for the sampling process, impacting the clarity and quality of the generated samples. Type should be `FLOAT`.
        - `denoise_seq` (Required): Specifies the denoising level for subsequent steps in the sequence, allowing for dynamic adjustment of clarity. Type should be `FLOAT`.
        - `unsample_latents` (Required): Determines whether to unsample latents during the sequence generation, affecting the detail and quality of the output. Type should be `BOOLEAN`.
        - `inject_noise` (Required): Enables the injection of noise into the latent space, introducing variability and texture to the generated samples. Type should be `BOOLEAN`.
        - `noise_strength` (Required): Specifies the strength of the noise to be injected, controlling the amount of variability introduced. Type should be `FLOAT`.
        - `denoise_sine` (Required): Enables sine wave modulation of the denoise parameter, creating dynamic changes in clarity throughout the sequence. Type should be `BOOLEAN`.
        - `denoise_max` (Required): Sets the maximum denoising level achievable through sine wave modulation, defining the upper limit of clarity. Type should be `FLOAT`.
        - `seed_keying` (Required): Enables seed keying to vary the seed based on specific conditions or modes, introducing further variability. Type should be `BOOLEAN`.
        - `seed_keying_mode` (Required): Specifies the mode of seed keying, affecting how the seed changes throughout the sequence. Type should be `COMBO[STRING]`.
        - `seed_divisor` (Required): Determines the divisor used in modulo seed keying, influencing the frequency of seed changes. Type should be `INT`.
    - Outputs:
        - `latent`: Represents the final generated sample or sequence of samples, encapsulating the result of the complex sampling process. Type should be `LATENT`.
