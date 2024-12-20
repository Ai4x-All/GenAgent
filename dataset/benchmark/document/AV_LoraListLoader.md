- `AV_LoraListLoader`: The AVLoraListLoader node is designed for loading and stacking lists of LoRA models based on provided data and configurations. It facilitates the dynamic enhancement of models and clips by applying multiple LoRA adjustments in sequence, allowing for complex model behavior modifications through LoRA parameters.
    - Inputs:
        - `model` (Required): The 'model' parameter represents the initial model to which LoRA adjustments will be applied. It is crucial for defining the starting point of the LoRA stacking process. Type should be `MODEL`.
        - `clip` (Required): The 'clip' parameter signifies the initial clip model that will be modified alongside the main model through the LoRA adjustments. It plays a key role in the stacking process by being subject to modifications. Type should be `CLIP`.
        - `data` (Required): The 'data' parameter contains the list of LoRA models to be loaded and applied, in JSON format. It is essential for specifying which LoRA models and their corresponding strengths will influence the model and clip. Type should be `STRING`.
        - `base_url` (Optional): The 'base_url' parameter provides the base URL for fetching LoRA models not found locally. It aids in dynamically loading LoRA models from external sources. Type should be `STRING`.
    - Outputs:
        - `model`: Returns the modified model after applying the specified LoRA adjustments. Type should be `MODEL`.
        - `clip`: Returns the modified clip model after the LoRA adjustments have been applied. Type should be `CLIP`.
