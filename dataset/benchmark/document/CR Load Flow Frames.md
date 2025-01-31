- `CR Load Flow Frames`: The node is designed to load sequential image frames for animation purposes, handling the initial frame differently if no frames are skipped and preparing both the current and previous frames for further processing.
    - Inputs:
        - `input_folder` (Required): The name of the folder from which the images will be loaded. This parameter is essential for identifying the specific directory containing the animation frames. Type should be `COMBO[STRING]`.
        - `sort_by` (Required): Determines the order in which the files are sorted before loading. This affects the sequence in which frames are processed and displayed. Type should be `COMBO[STRING]`.
        - `current_frame` (Required): Specifies the index of the current frame to be loaded, adjusting for any initial frames skipped. This index is crucial for determining the sequence of frames and ensuring the correct frame is processed next. Type should be `INT`.
        - `skip_start_frames` (Required): Indicates the number of initial frames to skip before starting the loading process. This parameter allows for flexibility in starting the animation from a specific frame. Type should be `INT`.
        - `input_path` (Optional): An optional specific path to a directory or file to be loaded. Overrides the default path constructed from the input directory and folder name. Type should be `STRING`.
        - `file_pattern` (Optional): A pattern to match specific files within the directory. This allows for filtering and loading only the files that match the given pattern. Type should be `STRING`.
    - Outputs:
        - `current_image`: The current image frame loaded and processed for animation. Type should be `IMAGE`.
        - `previous_image`: The previous image frame loaded and processed, used for comparison or reference in animation. Type should be `IMAGE`.
        - `current_frame`: The index of the current frame that has been loaded. Type should be `INT`.
        - `show_help`: A URL providing additional help and documentation related to the node. Type should be `STRING`.
