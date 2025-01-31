- `CheckpointNameSelector`: The CheckpointNameSelector node is designed to facilitate the selection of checkpoint names from a predefined list, streamlining the process of identifying and utilizing specific checkpoints within a workflow. It abstracts the complexity of navigating through checkpoint directories, offering a user-friendly interface for selecting the desired checkpoint name.
    - Inputs:
        - `ckpt_name` (Required): The 'ckpt_name' parameter allows users to specify the name of the checkpoint they wish to select. This selection is crucial as it determines which checkpoint will be utilized for subsequent operations, directly influencing the workflow's outcome. Type should be `COMBO[STRING]`.
    - Outputs:
        - `ckpt_name`: Returns the selected checkpoint name, enabling further processing or utilization within the workflow. Type should be `COMBO[STRING]`.
        - `ckpt_name_str`: Provides the selected checkpoint name as a string, facilitating its use in scenarios where a string representation is required. Type should be `STRING`.
