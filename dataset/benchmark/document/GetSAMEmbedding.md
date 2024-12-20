- `GetSAMEmbedding`: The GetSAMEmbedding node is designed to extract semantic embeddings from images using a specific SAM model. It facilitates the transformation of visual content into a format that can be further processed or analyzed, emphasizing the extraction of meaningful features that represent the underlying content of the images.
    - Inputs:
        - `sam_model` (Required): The SAM model used for generating embeddings from images. It plays a crucial role in determining the quality and relevance of the extracted features. Type should be `AV_SAM_MODEL`.
        - `image` (Required): The input image from which embeddings are to be extracted. This image is processed by the SAM model to generate a semantic representation. Type should be `IMAGE`.
        - `device_mode` (Optional): Specifies the computational device (AUTO, Prefer GPU, CPU) for model inference, affecting performance and resource utilization. Type should be `COMBO[STRING]`.
    - Outputs:
        - `sam_embedding`: The semantic embedding generated from the input image, representing its meaningful features in a condensed form. Type should be `SAM_EMBEDDING`.
