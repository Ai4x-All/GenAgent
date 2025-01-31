- `Inference_Core_DiffusionEdge_Preprocessor`: This node is designed to preprocess images for further processing by applying a diffusion edge detection algorithm. It enhances the edges in images based on the specified environment and patch batch size, making it suitable for tasks that require detailed edge information, such as line extraction in control networks.
    - Inputs:
        - `image` (Required): The input image to be processed by the diffusion edge detection algorithm. Type should be `IMAGE`.
        - `environment` (Optional): Specifies the environment setting for the edge detection model, affecting the model's behavior and the resulting edge enhancements. Type should be `COMBO[STRING]`.
        - `patch_batch_size` (Optional): Determines the number of image patches processed simultaneously, influencing the execution speed and memory usage. Type should be `INT`.
        - `resolution` (Optional): The resolution to which the input image is resized before processing, affecting the detail level of the detected edges. Type should be `INT`.
    - Outputs:
        - `image`: The processed image with enhanced edges, ready for further processing or visualization. Type should be `IMAGE`.
