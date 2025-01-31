- `IPAdapterStyleCompositionBatch`: The IPAdapterStyleCompositionBatch node is designed for advanced image processing, specifically focusing on blending and enhancing images through style and composition adjustments. It extends the capabilities of IPAdapterStyleComposition by allowing batch processing, enabling efficient handling of multiple images simultaneously.
    - Inputs:
        - `model` (Required): Specifies the model to be used for the image processing task, serving as the core computational element. Type should be `MODEL`.
        - `ipadapter` (Required): Defines the IPAdapter to be utilized, which is a key component in the image processing pipeline. Type should be `IPADAPTER`.
        - `image_style` (Required): The image to be used as the style reference in the composition process. Type should be `IMAGE`.
        - `image_composition` (Required): The image to be used for composition, acting as the base for style application. Type should be `IMAGE`.
        - `weight_style` (Required): Determines the influence of the style image on the final output, allowing for fine-tuned control over the style intensity. Type should be `FLOAT`.
        - `weight_composition` (Required): Controls the impact of the composition image on the final result, enabling precise adjustment of the composition effect. Type should be `FLOAT`.
        - `expand_style` (Required): A boolean flag that, when set to true, expands the style application across the composition, offering a broader stylistic influence. Type should be `BOOLEAN`.
        - `start_at` (Required): Defines the starting point of the effect application in the processing sequence, allowing for staged integration of styles and compositions. Type should be `FLOAT`.
        - `end_at` (Required): Sets the endpoint for the effect application, providing a boundary for style and composition adjustments. Type should be `FLOAT`.
        - `embeds_scaling` (Required): Specifies the method for scaling embeddings, which influences how style and composition features are integrated into the image. Type should be `COMBO[STRING]`.
        - `image_negative` (Optional): An optional image that serves as a negative influence, reducing its stylistic or compositional features in the final output. Type should be `IMAGE`.
        - `attn_mask` (Optional): An optional mask that directs attention to specific areas of the image, enhancing or diminishing effects accordingly. Type should be `MASK`.
        - `clip_vision` (Optional): Optionally integrates CLIP vision models to refine the style and composition effects based on semantic understanding. Type should be `CLIP_VISION`.
    - Outputs:
        - `model`: The modified model after processing the images with style and composition adjustments. Type should be `MODEL`.
