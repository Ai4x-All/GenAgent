- `ttN pipeEDIT`: The ttN pipeEDIT node is designed for editing and refining the parameters and settings of a pipeline, allowing for the customization and optimization of the pipeline's behavior and output. It focuses on enhancing the flexibility and control over the pipeline's execution by enabling adjustments to its components and configurations.
    - Inputs:
        - `pipe` (Optional): Represents the pipeline to be edited or refined, serving as the core structure for modification. It is crucial for determining the base configuration and elements that will undergo adjustments. Type should be `PIPE_LINE`.
        - `model` (Optional): Specifies the model component of the pipeline, allowing for its selection or modification. Type should be `MODEL`.
        - `pos` (Optional): Defines the positive conditioning aspect of the pipeline, enabling its specification or alteration. Type should be `CONDITIONING`.
        - `neg` (Optional): Specifies the negative conditioning component, allowing for adjustments to how the pipeline handles negative inputs. Type should be `CONDITIONING`.
        - `latent` (Optional): Represents the latent space configuration of the pipeline, permitting adjustments to its handling of latent variables. Type should be `LATENT`.
        - `vae` (Optional): Specifies the VAE (Variational Autoencoder) component, enabling its selection or modification within the pipeline. Type should be `VAE`.
        - `clip` (Optional): Defines the CLIP model component of the pipeline, allowing for its specification or alteration. Type should be `CLIP`.
        - `image` (Optional): Specifies the image component of the pipeline, enabling adjustments to how images are handled. Type should be `IMAGE`.
        - `seed` (Optional): Represents the seed value for random number generation within the pipeline, allowing for its specification to ensure reproducibility. Type should be `INT`.
    - Outputs:
        - `pipe`: Returns the modified pipeline, reflecting the applied edits and refinements. Type should be `PIPE_LINE`.
        - `model`: Outputs the selected or modified model component of the pipeline. Type should be `MODEL`.
        - `pos`: Outputs the specified or altered positive conditioning component of the pipeline. Type should be `CONDITIONING`.
        - `neg`: Outputs the adjusted negative conditioning component of the pipeline. Type should be `CONDITIONING`.
        - `latent`: Returns the adjusted latent space configuration of the pipeline. Type should be `LATENT`.
        - `vae`: Outputs the selected or modified VAE component of the pipeline. Type should be `VAE`.
        - `clip`: Outputs the specified or altered CLIP model component of the pipeline. Type should be `CLIP`.
        - `image`: Outputs the adjusted image component of the pipeline. Type should be `IMAGE`.
        - `seed`: Returns the specified seed value for random number generation within the pipeline. Type should be `INT`.