- `Inference_Core_OneFormer-ADE20K-SemSegPreprocessor`: This node is designed for semantic segmentation tasks using the OneFormer model specifically trained on the ADE20K dataset. It preprocesses images to facilitate semantic segmentation, leveraging a pretrained OneFormer model to analyze and segment the input image into different semantic categories based on the ADE20K dataset standards.
    - Parameters:
        - `resolution`: Specifies the resolution for the output image after segmentation. This affects the level of detail and size of the segmented output. Type should be `INT`.
    - Inputs:
        - `image`: The input image to be semantically segmented. This image is processed and segmented into different semantic categories using the OneFormer model. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output of the semantic segmentation process, which is an image segmented into different semantic categories. Type should be `IMAGE`.