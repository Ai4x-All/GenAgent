- `easy loraStack`: The `loraStackLoader` node is designed to dynamically load and manage LoRA (Low-Rank Adaptation) models for enhancing or modifying the behavior of neural networks. It allows for the flexible integration of multiple LoRA models, adjusting their strengths and applying them to specific components of a network, thereby enabling customized and efficient model adaptation.
    - Parameters:
        - `toggle`: Determines whether the LoRA stack loading functionality is enabled or disabled, affecting whether any LoRA models are loaded and applied. Type should be `COMBO[BOOLEAN]`.
        - `mode`: Specifies the operational mode of the node, which can influence how LoRA models are selected and utilized within the system. Type should be `COMBO[STRING]`.
        - `num_loras`: Defines the number of LoRA models to be loaded and managed by the node, allowing for the customization of the model adaptation process. Type should be `INT`.
        - `lora_i_name`: Specifies the name of the i-th LoRA model to be loaded, enabling the selection of specific models for application. Type should be `COMBO[STRING]`.
        - `lora_i_strength`: Defines the overall strength of the i-th LoRA model to be applied, affecting the intensity of its impact on the neural network. Type should be `FLOAT`.
        - `lora_i_model_strength`: Specifies the strength of the i-th LoRA model's effect on the model component of the neural network. Type should be `FLOAT`.
        - `lora_i_clip_strength`: Specifies the strength of the i-th LoRA model's effect on the CLIP component of the neural network. Type should be `FLOAT`.
    - Inputs:
        - `optional_lora_stack`: An optional parameter that allows for the inclusion of an existing stack of LoRA models to be considered in the loading process. Type should be `LORA_STACK`.
    - Outputs:
        - `lora_stack`: Outputs a collection of LoRA models that have been loaded and configured based on the input parameters, ready for integration into the target neural network. Type should be `LORA_STACK`.