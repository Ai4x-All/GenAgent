- `SetLatentNoiseMask`: This node is designed to apply a noise mask to a set of latent samples. It modifies the input samples by integrating a specified mask, thereby altering their noise characteristics.
    - Inputs:
        - `samples` (Required): The latent samples to which the noise mask will be applied. This parameter is crucial for determining the base content that will be modified. Type should be `LATENT`.
        - `mask` (Required): The mask to be applied to the latent samples. It defines the areas and intensity of noise alteration within the samples. Type should be `MASK`.
    - Outputs:
        - `latent`: The modified latent samples with the applied noise mask. Type should be `LATENT`.