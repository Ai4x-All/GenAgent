- `Checkpoint Loader (Simple)`: This node is designed to load checkpoints for models, specifically focusing on a simplified process that requires only the checkpoint name. It aims to streamline the loading of model states for further use or analysis, making it accessible even without specifying configuration details.
    - Parameters:
        - `ckpt_name`: The name of the checkpoint to be loaded. This parameter is crucial as it identifies the specific checkpoint file from which the model's state will be restored. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `MODEL`: The loaded model state. Type should be `MODEL`.
        - `CLIP`: The loaded CLIP model component, if applicable. Type should be `CLIP`.
        - `VAE`: The loaded VAE model component, if applicable. Type should be `VAE`.
        - `NAME_STRING`: The name string derived from the checkpoint, providing an identifier for the loaded model. Type should be `STRING`.