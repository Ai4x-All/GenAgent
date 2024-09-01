- `easy latentCompositeMaskedWithCond`: This node is designed for advanced image manipulation within the latent space, specifically tailored for conditional composite operations. It enables the blending of two latent representations based on a mask, with additional conditions that can modify the blending process. This functionality is crucial for creating nuanced and contextually aware modifications to generated images, allowing for precise control over the composition of visual elements.
    - Parameters:
        - `text_combine_mode`: unknown Type should be `COMBO[STRING]`.
        - `replace_text`: unknown Type should be `STRING`.
    - Inputs:
        - `pipe`: unknown Type should be `PIPE_LINE`.
        - `text_combine`: unknown Type should be `LIST`.
        - `source_latent`: unknown Type should be `LATENT`.
        - `source_mask`: unknown Type should be `MASK`.
        - `destination_mask`: unknown Type should be `MASK`.
    - Outputs:
        - `pipe`: unknown Type should be `PIPE_LINE`.
        - `latent`: unknown Type should be `LATENT`.
        - `conditioning`: unknown Type should be `CONDITIONING`.