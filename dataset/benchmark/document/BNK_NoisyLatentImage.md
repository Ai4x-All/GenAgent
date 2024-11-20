- `BNK_NoisyLatentImage`: The Noisy Latent Image node generates a tensor of random noise as latent images, configurable by dimensions and batch size, and intended for use in generative models where noise serves as a foundational element for image synthesis.
    - Inputs:
        - `source` (Required): Specifies the computational resource (CPU or GPU) to be used for generating the noise, affecting the execution speed and efficiency. Type should be `COMBO[STRING]`.
        - `seed` (Required): Determines the initialization value for random number generation, ensuring reproducibility of the noise patterns. Type should be `INT`.
        - `width` (Required): Sets the width of the generated latent images, influencing the dimensions of the output noise tensor. Type should be `INT`.
        - `height` (Required): Sets the height of the generated latent images, influencing the dimensions of the output noise tensor. Type should be `INT`.
        - `batch_size` (Required): Defines the number of latent images to generate in a single batch, allowing for batch processing of noise generation. Type should be `INT`.
    - Outputs:
        - `latent`: The generated tensor of random noise, structured as latent images for further processing or model input. Type should be `LATENT`.