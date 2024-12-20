- `Automatic CFG - Attention modifiers tester`: This node is designed to test and apply various attention modifier configurations to computational graph models, specifically focusing on enhancing or altering the attention mechanisms within these models. It aims to experiment with different attention modification strategies to optimize model performance or behavior.
    - Inputs:
        - `seed` (Required): Specifies the seed for random number generation, ensuring reproducibility of the attention modifier application. Type should be `INT`.
        - `sigma_start` (Required): Defines the starting value of sigma for the attention modifier, indicating the beginning of the range within which the modifier is active. Type should be `FLOAT`.
        - `sigma_end` (Required): Defines the ending value of sigma for the attention modifier, indicating the end of the range within which the modifier is active. Type should be `FLOAT`.
        - `self_attn_mod_eval` (Required): Contains the evaluation code for self-attention modification, allowing for dynamic adjustment of attention mechanisms based on the model's requirements. Type should be `STRING`.
        - `unet_block_id_input` (Required): Identifies the input block IDs where the attention modifier will be applied, enabling targeted modifications. Type should be `STRING`.
        - `unet_block_id_middle` (Required): Identifies the middle block IDs where the attention modifier will be applied, enabling targeted modifications. Type should be `STRING`.
        - `unet_block_id_output` (Required): Identifies the output block IDs where the attention modifier will be applied, enabling targeted modifications. Type should be `STRING`.
        - `unet_attn` (Required): Specifies the type of attention (self, cross, or both) to be modified, allowing for precise control over the modification process. Type should be `COMBO[STRING]`.
        - `join_parameters` (Optional): Allows for the combination of attention modifier parameters from another source, enhancing the flexibility of attention modification. Type should be `ATTNMOD`.
    - Outputs:
        - `Attention modifier`: Outputs the modified attention parameters, reflecting the changes made to the model's attention mechanisms. Type should be `ATTNMOD`.
        - `Parameters as string`: Provides a string representation of the attention modifier parameters, facilitating easy review and documentation of the modifications. Type should be `STRING`.
