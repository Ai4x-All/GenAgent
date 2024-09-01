- `ModelMergeSDXLTransformers`: This node specializes in merging the transformer blocks of two SDXL models, allowing for intricate customization of model behavior by adjusting the influence of specific transformer components across the models.
    - Parameters:
        - `time_embed.`: Adjusts the influence of the time embedding component in the merging process. Type should be `FLOAT`.
        - `label_emb.`: Adjusts the influence of the label embedding component in the merging process. Type should be `FLOAT`.
        - `input_blocks.i.j.`: unknown Type should be `FLOAT`.
        - `input_blocks.i.j.transformer_blocks.k.`: unknown Type should be `FLOAT`.
        - `middle_block.i.`: Adjusts the influence of the i-th middle block in the merging process. The index i ranges from 0 to 2. Type should be `FLOAT`.
        - `middle_block.i.transformer_blocks.j.`: unknown Type should be `FLOAT`.
        - `output_blocks.i.j.`: unknown Type should be `FLOAT`.
        - `output_blocks.i.j.transformer_blocks.k.`: unknown Type should be `FLOAT`.
        - `out.`: Adjusts the final output of the merging process. Type should be `FLOAT`.
    - Inputs:
        - `model1`: The first SDXL model to be merged. It serves as the base model for the merging process. Type should be `MODEL`.
        - `model2`: The second SDXL model to be merged. Its transformer blocks can be selectively blended into the first model. Type should be `MODEL`.
    - Outputs:
        - `model`: The resulting model after merging the specified components of the two SDXL models. Type should be `MODEL`.