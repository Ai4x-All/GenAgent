- `easy ipadapterApplyEmbeds`: This node is designed for applying embedding adjustments to models using IPAdapter, facilitating the integration of specific embeddings into the model's processing pipeline. It abstracts the complexity of embedding manipulation, offering a streamlined approach to enhance model performance with tailored embeddings.
    - Parameters:
        - `weight`: Specifies the weight of the embeddings in the adjustment process, influencing the degree to which the embeddings affect the model. Type should be `FLOAT`.
        - `weight_type`: Defines the type of weighting applied to the embeddings, affecting how they are integrated into the model. Type should be `COMBO[STRING]`.
        - `start_at`: The starting point in the model's layers or processing stages where the embeddings begin to be applied, determining the scope of their impact. Type should be `FLOAT`.
        - `end_at`: The ending point in the model's layers or processing stages where the embeddings cease to be applied, marking the limit of their influence. Type should be `FLOAT`.
        - `embeds_scaling`: Describes how the embeddings are scaled or adjusted before being applied, impacting the final embedding integration. Type should be `COMBO[STRING]`.
    - Inputs:
        - `model`: The model to which embeddings will be applied. It serves as the base for embedding adjustments, playing a crucial role in the node's operation. Type should be `MODEL`.
        - `ipadapter`: The IPAdapter instance used for embedding adjustments. It is essential for the node's functionality, enabling the precise application of embeddings. Type should be `IPADAPTER`.
        - `pos_embed`: The positive embeddings to be applied. These embeddings are crucial for adjusting the model's output in a desired direction, enhancing its performance. Type should be `EMBEDS`.
        - `neg_embed`: The negative embeddings that can be optionally applied to counterbalance or adjust the model's output in the opposite direction. Type should be `EMBEDS`.
        - `attn_mask`: An optional attention mask that can be applied during the embedding adjustment process, focusing the embedding's impact on specific parts of the input. Type should be `MASK`.
    - Outputs:
        - `model`: The model after applying the embeddings. It reflects the adjustments made using the specified embeddings, showcasing the node's capability to enhance model performance. Type should be `MODEL`.
        - `ipadapter`: The IPAdapter instance after embedding adjustments. It indicates the successful application of embeddings, essential for the node's functionality. Type should be `IPADAPTER`.