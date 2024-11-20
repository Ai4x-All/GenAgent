- `STMFNet VFI`: The STMFNet VFI node is designed for video frame interpolation, leveraging deep learning models to predict and generate intermediate frames between existing frames in a video sequence. It utilizes a combination of extraction, decoding, and refining processes to enhance the temporal resolution of videos by filling in missing frames with high accuracy and visual quality.
    - Inputs:
        - `ckpt_name` (Required): Specifies the checkpoint name for the STMFNet model to be loaded, crucial for initializing the model with pre-trained weights. Type should be `COMBO[STRING]`.
        - `frames` (Required): The sequence of frames to be interpolated, serving as the input video data for frame interpolation. Type should be `IMAGE`.
        - `clear_cache_after_n_frames` (Required): Determines after how many frames the CUDA cache should be cleared to manage memory usage effectively. Type should be `INT`.
        - `multiplier` (Required): Defines the factor by which the frame rate is increased, currently fixed to 2x interpolation. Type should be `INT`.
        - `duplicate_first_last_frames` (Required): A boolean flag to indicate whether the first and last frames should be duplicated, affecting the output frame sequence. Type should be `BOOLEAN`.
        - `optional_interpolation_states` (Optional): Optional states to manage frame skipping during interpolation, providing flexibility in handling specific frames. Type should be `INTERPOLATION_STATES`.
    - Outputs:
        - `image`: The output of the node, consisting of the interpolated video frames, enhancing the video's temporal resolution. Type should be `IMAGE`.