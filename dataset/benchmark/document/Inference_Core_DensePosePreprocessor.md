- `Inference_Core_DensePosePreprocessor`: The DensePose Preprocessor node is designed to estimate human body poses and overlay them on images using DensePose models. It supports different models and color maps for visualization, providing a flexible approach to pose estimation and visualization.
    - Inputs:
        - `image` (Required): The input image on which body poses will be estimated and visualized. Type should be `IMAGE`.
        - `model` (Optional): Specifies the DensePose model to be used for pose estimation. The choice of model can affect the accuracy and performance of pose estimation. Type should be `COMBO[STRING]`.
        - `cmap` (Optional): Determines the color map used for visualizing the pose estimation results. Different color maps can be used to enhance the visual distinction of pose estimations. Type should be `COMBO[STRING]`.
        - `resolution` (Optional): The resolution to which the input image is resized before pose estimation. Affects the detail level of the pose estimation. Type should be `INT`.
    - Outputs:
        - `image`: The output is an image with human body poses estimated and visualized on it. Type should be `IMAGE`.