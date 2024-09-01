- `CheckpointNameSelector`: The CheckpointNameSelector node is designed to facilitate the selection of checkpoint names from a predefined list, streamlining the process of identifying and utilizing specific checkpoints within a workflow.
    - Parameters:
        - `ckpt_name`: Specifies the name of the checkpoint to be selected. This parameter is crucial for determining which checkpoint is to be utilized in subsequent operations. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `ckpt_name`: Returns the selected checkpoint name, enabling its use in further processing or operations. Type should be `COMBO[STRING]`.
        - `ckpt_name_str`: Provides the selected checkpoint name as a string, facilitating its integration into workflows that require textual representation. Type should be `STRING`.