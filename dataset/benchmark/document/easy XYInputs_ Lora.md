- `easy XYInputs_ Lora`: This node is designed to facilitate the generation and manipulation of XY plot values based on Lora configurations. It dynamically adjusts model and clip strengths for each Lora, optionally incorporating weights and allowing for the extension of Lora configurations through an optional stack. The node aims to provide a flexible interface for visualizing and customizing Lora-based data representations.
    - Inputs:
        - `input_mode` (Required): Specifies the mode of input, determining whether weights are included in the Lora configurations. It affects how the node processes and generates XY plot values. Type should be `COMBO[STRING]`.
        - `lora_count` (Required): Defines the number of Loras to be considered for generating XY plot values. It directly influences the size and complexity of the output data. Type should be `INT`.
        - `model_strength` (Required): Sets a default or specific model strength for each Lora, used as a baseline unless overridden by individual Lora configurations. Type should be `FLOAT`.
        - `clip_strength` (Required): Determines a default or specific clip strength for each Lora, serving as a baseline unless individual Lora configurations specify otherwise. Type should be `FLOAT`.
        - `lora_name_i` (Required): Specifies the name of each Lora, allowing for individual identification and configuration within the XY plot generation process. Type should be `COMBO[STRING]`.
        - `model_str_i` (Required): Sets the model strength for each Lora individually, overriding the default model strength if specified. Type should be `FLOAT`.
        - `clip_str_i` (Required): Sets the clip strength for each Lora individually, overriding the default clip strength if specified. Type should be `FLOAT`.
        - `optional_lora_stack` (Optional): Allows for the extension of Lora configurations beyond the specified count, enabling more complex and customized data representations. Type should be `LORA_STACK`.
    - Outputs:
        - `X or Y`: Represents the generated XY plot values based on the provided Lora configurations, ready for visualization or further processing. Type should be `X_Y`.
