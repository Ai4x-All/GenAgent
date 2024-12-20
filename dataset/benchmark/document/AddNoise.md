- `AddNoise`: The AddNoise node introduces controlled noise to latent images in a generative model's sampling process, enhancing the diversity or realism of generated samples.
    - Inputs:
        - `model` (Required): The generative model for which noise is being added. It plays a crucial role in the noise addition process by providing model-specific operations for processing latent images. Type should be `MODEL`.
        - `noise` (Required): A noise generator object responsible for creating noise to be added to the latent images. Type should be `NOISE`.
        - `sigmas` (Required): A sequence of sigma values determining the scale of noise to be added. It influences the intensity and variation of the noise applied. Type should be `SIGMAS`.
        - `latent_image` (Required): The latent image to which noise will be added. It serves as the base for noise application, affecting the final output. Type should be `LATENT`.
    - Outputs:
        - `latent`: The modified latent image after noise has been added, reflecting the impact of the noise addition process. Type should be `LATENT`.
