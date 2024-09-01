- `VHS_VideoCombine`: The VHS_VideoCombine node is designed to facilitate the combination of various video elements into a single cohesive output. It abstracts the complexities involved in merging video streams, audio tracks, and potentially other multimedia components, aiming to streamline the process of video production and editing within the Video Helper Suite environment.
    - Parameters:
        - `frame_rate`: Specifies the playback speed of the resulting video in frames per second, influencing the smoothness of motion. Type should be `FLOAT`.
        - `loop_count`: Determines how many times the video loops. A value of 0 indicates infinite looping. Type should be `INT`.
        - `filename_prefix`: The prefix for the output file names, allowing for easy identification and organization of generated videos. Type should be `STRING`.
        - `format`: Defines the output video format, including options like GIF, WEBP, and various formats supported by ffmpeg. Type should be `COMBO[STRING]`.
        - `pingpong`: Enables or disables the pingpong effect, where the video plays forwards then backwards, creating a seamless loop effect. Type should be `BOOLEAN`.
        - `save_output`: Controls whether the output video is saved to disk, enabling further processing or direct use. Type should be `BOOLEAN`.
    - Inputs:
        - `images`: A sequence of images to be combined into a video. This is the primary visual content of the output video. Type should be `IMAGE`.
        - `audio`: Optional audio track to be included in the video output, enhancing the multimedia experience. Type should be `VHS_AUDIO`.
        - `meta_batch`: Manages batch processing of video data, facilitating efficient handling of multiple video operations. Type should be `VHS_BatchManager`.
    - Outputs:
        - `Filenames`: The filenames of the generated video files, providing a direct reference to the output for further use or distribution. Type should be `VHS_FILENAMES`.