- `easy unSampler`: The `easy unSampler` node is designed for the reverse sampling process in generative models, allowing for the exploration of latent spaces and the refinement of generated images by stepping back through the model's layers. It provides a flexible interface for adjusting the sampling parameters and integrating with different sampler and scheduler types.
    - Inputs:
        - `steps` (Required): Specifies the number of steps to take in the reverse sampling process, affecting the granularity of the exploration or refinement. Type should be `INT`.
        - `end_at_step` (Required): Determines the final step of the reverse sampling process, enabling partial reversals and targeted refinement. Type should be `INT`.
        - `cfg` (Required): Controls the conditioning factor, influencing the strength of conditioning on the input prompt or image features during reverse sampling. Type should be `FLOAT`.
        - `sampler_name` (Required): Selects the specific sampler to use for the reverse sampling process, allowing for customization of the sampling strategy. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): Chooses the scheduler for controlling the sampling steps, impacting the progression and dynamics of the reverse sampling. Type should be `COMBO[STRING]`.
        - `normalize` (Required): Enables or disables normalization, affecting the handling of input data and the stability of the reverse sampling process. Type should be `COMBO[STRING]`.
        - `pipe` (Optional): The pipeline configuration for the reverse sampling process, including model and conditioning settings. Type should be `PIPE_LINE`.
        - `optional_model` (Optional): Optionally specifies a model to use for the reverse sampling, overriding the default. Type should be `MODEL`.
        - `optional_positive` (Optional): Optionally adds positive conditioning to the reverse sampling process. Type should be `CONDITIONING`.
        - `optional_negative` (Optional): Optionally adds negative conditioning to the reverse sampling process. Type should be `CONDITIONING`.
        - `optional_latent` (Optional): Optionally specifies a latent representation to use as a starting point for the reverse sampling. Type should be `LATENT`.
    - Outputs:
        - `pipe`: Returns the modified pipeline after the reverse sampling process, including any changes to the latent space or generated images. Type should be `PIPE_LINE`.
        - `latent`: Outputs the latent representation obtained or modified during the reverse sampling process, providing insight into the model's internal state. Type should be `LATENT`.
