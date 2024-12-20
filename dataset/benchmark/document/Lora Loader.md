- `Lora Loader`: The LoraLoader node is designed to dynamically load and apply LoRA (Low-Rank Adaptation) adjustments to given models and CLIP instances, enhancing their capabilities or altering their behavior based on specified LoRA parameters and strengths.
    - Inputs:
        - `model` (Required): The model to which the LoRA adjustments will be applied. It's crucial for defining the base architecture that will be enhanced or modified. Type should be `MODEL`.
        - `clip` (Required): The CLIP instance to which the LoRA adjustments will be applied, allowing for modifications in its behavior or performance. Type should be `CLIP`.
        - `lora_name` (Required): The name of the LoRA file containing the adjustments to be applied. It determines the specific LoRA modifications that will be loaded and applied. Type should be `COMBO[STRING]`.
        - `strength_model` (Required): Defines the intensity of the LoRA adjustments applied to the model. It influences how significantly the model's behavior is altered. Type should be `FLOAT`.
        - `strength_clip` (Required): Defines the intensity of the LoRA adjustments applied to the CLIP instance. It influences how significantly the CLIP's behavior is altered. Type should be `FLOAT`.
    - Outputs:
        - `MODEL`: The model with applied LoRA adjustments, reflecting enhanced or altered capabilities. Type should be `MODEL`.
        - `CLIP`: The CLIP instance with applied LoRA adjustments, reflecting modifications in behavior or performance. Type should be `CLIP`.
        - `NAME_STRING`: The name of the LoRA file applied, providing a reference to the specific adjustments made. Type should be `STRING`.
