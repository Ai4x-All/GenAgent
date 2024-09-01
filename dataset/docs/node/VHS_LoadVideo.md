- `VHS_LoadVideo`: The VHS_LoadVideo node is designed to facilitate the uploading and processing of video files within the Video Helper Suite. It handles the intricacies of loading video data from user uploads, ensuring compatibility and readiness for further processing or analysis within the suite.
    - Parameters:
        - `video`: Specifies the video file to be uploaded and processed. This parameter is crucial as it determines the video content that will undergo subsequent operations within the node. Type should be `COMBO[STRING]`.
        - `force_rate`: Defines the frame rate to which the video should be forced, allowing control over playback speed and frame sampling. Type should be `INT`.
        - `force_size`: Allows for the specification of a target size for the video, enabling resizing operations to adapt the video to certain dimensions or constraints. Type should be `COMBO[STRING]`.
        - `custom_width`: Sets a specific width for the video when resizing, providing flexibility in adjusting video dimensions. Type should be `INT`.
        - `custom_height`: Sets a specific height for the video when resizing, offering control over the vertical dimension of the video. Type should be `INT`.
        - `frame_load_cap`: Limits the number of frames to be loaded from the video, useful for processing or analyzing only a portion of the video. Type should be `INT`.
        - `skip_first_frames`: Skips a specified number of initial frames, useful for starting the processing at a later point in the video. Type should be `INT`.
        - `select_every_nth`: Selects every nth frame from the video, enabling downsampling for efficiency or specific analysis needs. Type should be `INT`.
    - Inputs:
        - `meta_batch`: Associates the video processing task with a specific batch manager, facilitating organized and efficient handling of multiple video processing tasks. Type should be `VHS_BatchManager`.
    - Outputs:
        - `IMAGE`: Represents the processed video frames, converted and ready for use within the suite's workflow. Type should be `IMAGE`.
        - `frame_count`: Provides the total number of frames in the uploaded video, useful for indexing and processing operations. Type should be `INT`.
        - `audio`: Extracts and outputs the audio track from the uploaded video, allowing for separate audio processing or analysis. Type should be `VHS_AUDIO`.
        - `video_info`: Gathers and outputs detailed information about the video, such as dimensions and duration, essential for further processing steps. Type should be `VHS_VIDEOINFO`.