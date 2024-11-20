- `IPAdapterWeights`: The IPAdapterWeights node is designed to manage and manipulate weights within the IPAdapter framework, focusing on the application of weight strategies for image processing. It enables the customization of weight distribution across frames, supports various timing methods, and facilitates the integration of images with weight-based adjustments.
    - Inputs:
        - `weights` (Required): A string of comma or newline-separated weight values to be converted into a list of floats. It forms the basis for weight distribution and manipulation. Type should be `STRING`.
        - `timing` (Required): Specifies the timing strategy for applying weights across frames, influencing the animation or transition effect. Type should be `COMBO[STRING]`.
        - `frames` (Required): The total number of frames to which the weights will be applied, defining the scope of the animation or transition. Type should be `INT`.
        - `start_frame` (Required): The starting frame number from which weight application begins, allowing for precise control over the animation's commencement. Type should be `INT`.
        - `end_frame` (Required): The ending frame number at which weight application concludes, marking the animation's termination point. Type should be `INT`.
        - `add_starting_frames` (Required): The number of additional frames to be added at the beginning of the animation, extending its start. Type should be `INT`.
        - `add_ending_frames` (Required): The number of additional frames to be added at the end of the animation, extending its duration. Type should be `INT`.
        - `method` (Required): The method used for applying weights across frames, affecting the pattern and distribution of weight adjustments. Type should be `COMBO[STRING]`.
        - `image` (Optional): An optional image input that, if provided, can be used in conjunction with weights for enhanced image processing effects. Type should be `IMAGE`.
    - Outputs:
        - `weights`: The processed list of weight values after applying the specified strategy and adjustments. Type should be `FLOAT`.
        - `weights_invert`: The inverted list of weight values, providing an alternative distribution for certain processing effects. Type should be `FLOAT`.
        - `total_frames`: The total number of frames resulting from the applied weight strategy, including any added starting or ending frames. Type should be `INT`.
        - `image_1`: The first image output, modified according to the weight strategy and method applied. Type should be `IMAGE`.
        - `image_2`: The second image output, modified in relation to the first image and the applied weight strategy. Type should be `IMAGE`.
        - `weights_strategy`: The weight strategy applied, encapsulating all weight-related parameters and their effects on the output. Type should be `WEIGHTS_STRATEGY`.