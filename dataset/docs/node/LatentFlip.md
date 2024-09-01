- `LatentFlip`: The LatentFlip node is designed to manipulate latent representations by flipping them either vertically or horizontally. This operation allows for the transformation of the latent space, potentially uncovering new variations or perspectives within the data.
    - Parameters:
        - `flip_method`: The 'flip_method' parameter specifies the axis along which the latent samples will be flipped. It can be either 'x-axis: vertically' or 'y-axis: horizontally', determining the direction of the flip and thus the nature of the transformation applied to the latent representations. Type should be `COMBO[STRING]`.
    - Inputs:
        - `samples`: The 'samples' parameter represents the latent representations to be flipped. The flipping operation alters these representations, either vertically or horizontally, depending on the 'flip_method' parameter, thus transforming the data in the latent space. Type should be `LATENT`.
    - Outputs:
        - `latent`: The output is a modified version of the input latent representations, having been flipped according to the specified method. This transformation can introduce new variations within the latent space. Type should be `LATENT`.