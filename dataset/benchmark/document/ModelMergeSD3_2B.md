- `ModelMergeSD3_2B`: This node specializes in merging two models by adjusting their embedding and block parameters specifically for the SD3_2B architecture. It allows for fine-tuned control over the merging process by providing adjustable parameters for positional, context, and various embedder components, as well as for each of the joint blocks and the final layer, enabling a highly customized integration of model features.
    - Inputs:
        - `model1` (Required): The first model to be merged. It serves as the base model for the merging process. Type should be `MODEL`.
        - `model2` (Required): The second model to be merged. Its features will be integrated into the first model based on the specified ratios. Type should be `MODEL`.
        - `pos_embed.` (Required): Adjusts the merging ratio for the positional embedding parameters, influencing how positional information is integrated from both models. Type should be `FLOAT`.
        - `x_embedder.` (Required): Controls the merging ratio for the x embedder, affecting the integration of x-axis positional information. Type should be `FLOAT`.
        - `context_embedder.` (Required): Determines the merging ratio for the context embedder, impacting how contextual information is blended between the two models. Type should be `FLOAT`.
        - `y_embedder.` (Required): Sets the merging ratio for the y embedder, influencing the integration of y-axis positional information. Type should be `FLOAT`.
        - `t_embedder.` (Required): Adjusts the merging ratio for the time embedder, affecting how temporal information is merged. Type should be `FLOAT`.
        - `joint_blocks.i.` (Required): unknown Type should be `FLOAT`.
        - `final_layer.` (Required): Controls the merging ratio for the final layer, determining how the final output features are combined. Type should be `FLOAT`.
    - Outputs:
        - `model`: The resulting model after merging, incorporating adjustments from both input models according to the specified ratios. Type should be `MODEL`.
