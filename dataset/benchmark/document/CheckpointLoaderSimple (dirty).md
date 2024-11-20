- `CheckpointLoaderSimple (dirty)`: This node simplifies the process of loading model checkpoints by automatically finding and loading the appropriate checkpoint file based on a given checkpoint name. It abstracts away the complexities of locating and verifying checkpoint files, making it easier to load models for further use or analysis.
    - Inputs:
        - `ckpt_name` (Required): Specifies the name of the checkpoint file to load. This parameter is crucial for identifying and retrieving the correct checkpoint file from a predefined list of available checkpoints. Type should be `STRING`.
    - Outputs:
        - `model`: Returns the loaded model from the specified checkpoint. Type should be `MODEL`.
        - `clip`: Returns the CLIP model associated with the loaded checkpoint, if available. Type should be `CLIP`.
        - `vae`: Returns the VAE model associated with the loaded checkpoint, if available. Type should be `VAE`.