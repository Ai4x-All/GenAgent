- `ADE_RawSigmaSchedule`: This node is designed to generate a sigma schedule based on a given beta schedule. It translates the beta schedule into a sigma schedule, which is essential for controlling the noise levels in diffusion models, particularly in the context of animation and image synthesis.
    - Inputs:
        - `raw_beta_schedule` (Required): Specifies the beta schedule to be converted into a sigma schedule. This parameter is crucial for determining the progression and intensity of noise levels throughout the diffusion process. Type should be `COMBO[STRING]`.
        - `linear_start` (Required): Defines the starting point of the linear interpolation used in the sigma schedule generation. It affects the initial noise level in the diffusion process. Type should be `FLOAT`.
        - `linear_end` (Required): Sets the endpoint for the linear interpolation in the sigma schedule, influencing the final noise level in the diffusion process. Type should be `FLOAT`.
        - `sampling` (Required): Determines the sampling method to be used in the sigma schedule, affecting how the noise levels are interpolated and applied. The type 'ModelSamplingType' should be understood as a placeholder for the actual sampling method chosen. Type should be `COMBO[STRING]`.
        - `lcm_original_timesteps` (Required): Specifies the number of original timesteps to be considered when using LCM sampling, impacting the granularity of the sigma schedule. Type should be `INT`.
        - `lcm_zsnr` (Required): A boolean flag indicating whether to apply Zero-SNR (zSNR) adjustments to the sigma schedule, enhancing the schedule's compatibility with certain diffusion processes. Type should be `BOOLEAN`.
    - Outputs:
        - `sigma_schedule`: The generated sigma schedule, which outlines the specific noise levels to be applied at each step of the diffusion process. Type should be `SIGMA_SCHEDULE`.
