- `easy styleAlignedBatchAlign`: The `easy styleAlignedBatchAlign` node is designed to apply style alignment to a batch of models, adjusting their normalization and attention mechanisms based on shared parameters. This process enhances the consistency and harmony of styles across different models, facilitating more cohesive and aesthetically pleasing outputs.
    - Inputs:
        - `model` (Required): The model parameter represents the neural network model to which style alignment will be applied. It is crucial for defining the base structure that will undergo normalization and attention adjustments. Type should be `MODEL`.
        - `share_norm` (Required): This parameter specifies how normalization layers within the model should be shared or aligned, impacting the overall style consistency and coherence of the model's output. Type should be `COMBO[STRING]`.
        - `share_attn` (Required): Determines the sharing strategy for attention mechanisms within the model, influencing how style elements are integrated and harmonized across different parts of the model. Type should be `COMBO[STRING]`.
        - `scale` (Required): Affects the intensity of style application, allowing for fine-tuning of the style's impact on the model's output. Type should be `FLOAT`.
    - Outputs:
        - `model`: The output is a modified version of the input model, now with adjusted normalization and attention mechanisms for enhanced style alignment. Type should be `MODEL`.