- `BNK_SlerpLatent`: The BNK_SlerpLatent node performs spherical linear interpolation (SLERP) between two latent spaces, allowing for smooth transitions and interpolations between different latent representations. It can optionally apply a mask to selectively interpolate parts of the latent spaces.
    - Parameters:
        - `factor`: A scalar factor determining the interpolation's progress between the two latent spaces. A factor of 0 returns the first latent space, while a factor of 1 returns the second. Type should be `FLOAT`.
    - Inputs:
        - `latents1`: The first set of latent representations to interpolate from. It serves as the starting point for the interpolation process. Type should be `LATENT`.
        - `latents2`: The second set of latent representations to interpolate towards. This optional parameter allows for interpolation between two distinct latent spaces. Type should be `LATENT`.
        - `mask`: An optional mask to apply during interpolation, enabling selective blending of the latent spaces based on the mask's pattern. Type should be `MASK`.
    - Outputs:
        - `latent`: The interpolated latent representation, smoothly blending between the two input latent spaces according to the specified factor and optional mask. Type should be `LATENT`.