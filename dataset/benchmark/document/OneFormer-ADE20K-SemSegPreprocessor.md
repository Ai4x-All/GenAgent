- `OneFormer-ADE20K-SemSegPreprocessor`: This node is designed for semantic segmentation tasks using the OneFormer model pre-trained on the ADE20K dataset. It processes images to segment them semantically, identifying and categorizing each pixel into a predefined class based on the ADE20K dataset.
    - Inputs:
        - `image` (Required): The input image to be semantically segmented. This image is processed by the OneFormer model to identify and categorize each pixel. Type should be `IMAGE`.
        - `resolution` (Optional): The resolution to which the input image is resized before processing. This affects the detail level of the segmentation output. Type should be `INT`.
    - Outputs:
        - `image`: The output of the semantic segmentation process. It is an image where each pixel is categorized into a class based on the ADE20K dataset. Type should be `IMAGE`.
