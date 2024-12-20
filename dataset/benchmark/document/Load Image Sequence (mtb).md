- `Load Image Sequence (mtb)`: The Load Image Sequence node is designed for loading sequences of images from a specified directory, allowing for the dynamic retrieval of individual frames or batches of frames based on the current frame index or a specified range. It supports loading all frames at once or fetching specific frames, making it versatile for applications requiring sequential image processing or animation.
    - Inputs:
        - `path` (Required): Specifies the directory path where the image sequence is stored. This path is crucial for locating and loading the desired images. Type should be `STRING`.
        - `current_frame` (Required): Determines the specific frame to load from the sequence. Setting this to -1 instructs the node to load all frames available, facilitating batch processing or full sequence retrieval. Type should be `INT`.
        - `range` (Optional): Defines a specific range of frames to load from the sequence, offering fine-grained control over which images are retrieved for processing. Type should be `STRING`.
    - Outputs:
        - `image`: The loaded image or images from the specified sequence. This output can be a single frame or a batch of frames, depending on the input parameters. Type should be `IMAGE`.
        - `mask`: The corresponding mask or masks for the loaded image(s), providing additional data for processing or analysis. Type should be `MASK`.
        - `current_frame`: The index of the current frame that was loaded, useful for tracking progress through a sequence. Type should be `INT`.
        - `total_frames`: The total number of frames loaded, which can be used to understand the scope of the sequence being processed. Type should be `INT`.
