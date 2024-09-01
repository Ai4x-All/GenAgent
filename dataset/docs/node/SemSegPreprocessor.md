- `SemSegPreprocessor`: The SemSegPreprocessor node is designed for preprocessing images for semantic segmentation tasks. It utilizes the UniFormer model to perform semantic segmentation, transforming input images into segmented outputs that categorize each pixel according to its semantic class. This node serves as a crucial step in preparing images for further analysis or model training within the domain of semantic segmentation.
    - Parameters:
        - `resolution`: Specifies the resolution to which the input image is resized before semantic segmentation. This parameter affects the granularity of the segmentation output, with higher resolutions potentially leading to more detailed segmentations. Type should be `INT`.
    - Inputs:
        - `image`: The input image to be processed for semantic segmentation. This parameter is crucial as it represents the raw data that will be transformed into a semantically segmented image, enabling further analysis or model training. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output of the semantic segmentation process. This is a segmented version of the input image, where each pixel is categorized according to its semantic class. Type should be `IMAGE`.