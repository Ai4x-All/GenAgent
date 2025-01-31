- `CheckpointLoader (dirty)`: This node is designed to load model checkpoints in a flexible manner, accommodating potentially mismatched or loosely specified checkpoint and configuration names. It utilizes utility functions to find the best match for given checkpoint and configuration names within a specified directory, thereby streamlining the process of loading models for further use or analysis.
    - Inputs:
        - `config_name` (Required): Specifies the configuration name to be used in conjunction with the checkpoint. The node attempts to find a matching configuration file name, enhancing flexibility in specifying configurations. Type should be `STRING`.
        - `ckpt_name` (Required): Indicates the checkpoint name to be loaded. The node employs utility functions to resolve the exact checkpoint file, allowing for a more lenient specification of checkpoint names. Type should be `STRING`.
    - Outputs:
        - `model`: Returns the loaded model object, ready for use in downstream tasks or analyses. Type should be `MODEL`.
        - `clip`: Returns the CLIP model associated with the loaded checkpoint, if applicable and requested. Type should be `CLIP`.
        - `vae`: Returns the VAE model associated with the loaded checkpoint, if applicable and requested. Type should be `VAE`.
