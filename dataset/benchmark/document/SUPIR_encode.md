- `SUPIR_encode`: The SUPIR_encode node is designed for encoding images into a latent space representation using a specified VAE model. It supports both standard and tiled encoding methods, allowing for flexible adaptation to different image sizes and computational constraints.
    - Inputs:
        - `SUPIR_VAE` (Required): The VAE model used for encoding the image. This model dictates the encoding process and the structure of the generated latent space. Type should be `SUPIRVAE`.
        - `image` (Required): The image to be encoded. This input is the primary data that the node processes to produce a latent representation. Type should be `IMAGE`.
        - `use_tiled_vae` (Required): A flag indicating whether to use a tiled approach for VAE encoding, which can be beneficial for processing large images or for reducing memory usage. Type should be `BOOLEAN`.
        - `encoder_tile_size` (Required): The size of the tiles used in the tiled VAE encoding process. This parameter is relevant only if 'use_tiled_vae' is True. Type should be `INT`.
        - `encoder_dtype` (Required): Specifies the data type for the encoder's output, allowing for control over the precision and size of the generated latent representation. Type should be `COMBO[STRING]`.
    - Outputs:
        - `latent`: The latent space representation of the encoded image. This output is crucial for further processing or generation tasks within the VAE framework. Type should be `LATENT`.