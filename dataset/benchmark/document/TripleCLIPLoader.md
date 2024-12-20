- `TripleCLIPLoader`: The TripleCLIPLoader node is designed for loading three distinct CLIP models simultaneously, facilitating advanced applications that require the integration of multiple CLIP embeddings or features for enhanced content understanding or generation.
    - Inputs:
        - `clip_name1` (Required): Specifies the first CLIP model to load, playing a crucial role in the composite CLIP model setup by contributing its unique embeddings or features. Type should be `COMBO[STRING]`.
        - `clip_name2` (Required): Defines the second CLIP model to load, adding another layer of complexity and capability to the overall CLIP model integration. Type should be `COMBO[STRING]`.
        - `clip_name3` (Required): Indicates the third CLIP model to load, further enriching the integrated CLIP model's ability to understand or generate content with diverse embeddings or features. Type should be `COMBO[STRING]`.
    - Outputs:
        - `clip`: Outputs a composite CLIP model that integrates the embeddings or features from the three loaded CLIP models, enabling advanced content understanding or generation tasks. Type should be `CLIP`.
