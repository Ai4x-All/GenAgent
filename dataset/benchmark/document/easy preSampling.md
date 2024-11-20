- `easy preSampling`: The 'easy preSampling' node is designed to configure and initiate a pre-sampling process, optimizing the input data before it undergoes further processing or model inference. This node abstracts the complexity of pre-sampling settings, allowing users to easily adjust parameters for improved model performance or data quality.
    - Inputs:
        - `pipe` (Required): Specifies the pipeline configuration for the pre-sampling process, determining the sequence of operations and models to be applied. Type should be `PIPE_LINE`.
        - `steps` (Required): Defines the number of steps to be executed in the pre-sampling process, affecting the depth of sampling and refinement. Type should be `INT`.
        - `cfg` (Required): Adjusts the conditioning factor, influencing the guidance and direction of the pre-sampling process. Type should be `FLOAT`.
        - `sampler_name` (Required): Selects the specific sampler algorithm to be used in the pre-sampling process, tailoring the sampling strategy. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): Chooses the scheduler for controlling the sampling process, managing the progression through steps. Type should be `COMBO[STRING]`.
        - `denoise` (Required): Sets the denoising level applied during the pre-sampling, enhancing the clarity and quality of the output. Type should be `FLOAT`.
        - `seed` (Required): Provides a seed value for the random number generator, ensuring reproducibility of the pre-sampling process. Type should be `INT`.
        - `image_to_latent` (Optional): Converts an input image to a latent representation, preparing it for further processing in the pre-sampling stage. Type should be `IMAGE`.
        - `latent` (Optional): Specifies the initial latent space representation to be used or modified during the pre-sampling process. Type should be `LATENT`.
    - Outputs:
        - `pipe`: The output pipeline configuration, reflecting any adjustments or transformations applied during the pre-sampling process. Type should be `PIPE_LINE`.