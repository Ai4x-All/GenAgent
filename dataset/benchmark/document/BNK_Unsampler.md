- `BNK_Unsampler`: The Unsampler node is designed to reverse the sampling process in generative models, allowing for the manipulation or refinement of latent images through specific configurations and steps. It integrates with various sampling and scheduling strategies to achieve desired outcomes.
    - Inputs:
        - `model` (Required): Specifies the generative model to be used for the unsampling process, central to determining the transformation applied to the latent image. Type should be `MODEL`.
        - `steps` (Required): Defines the number of steps to execute in the unsampling process, directly impacting the extent of transformation. Type should be `INT`.
        - `end_at_step` (Required): Specifies the final step at which the unsampling should conclude, allowing for partial unsampling sequences. Type should be `INT`.
        - `cfg` (Required): Configuration parameter influencing the unsampling behavior, potentially adjusting aspects like strength or direction of the process. Type should be `FLOAT`.
        - `sampler_name` (Required): Determines the sampling strategy to be employed, affecting how the latent image is processed during unsampling. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): Selects the scheduling algorithm to control the progression of steps in the unsampling process. Type should be `COMBO[STRING]`.
        - `normalize` (Required): Indicates whether to apply normalization to the latent image during unsampling, affecting the output's characteristics. Type should be `COMBO[STRING]`.
        - `positive` (Required): Positive conditioning text to guide the unsampling towards generating specific features or themes in the output. Type should be `CONDITIONING`.
        - `negative` (Required): Negative conditioning text to steer the unsampling away from certain features or themes, refining the output. Type should be `CONDITIONING`.
        - `latent_image` (Required): The initial latent image to be transformed through the unsampling process, serving as the starting point. Type should be `LATENT`.
    - Outputs:
        - `latent`: The transformed latent image resulting from the unsampling process, reflecting the applied configurations and steps. Type should be `LATENT`.