- `Write to GIF`: The 'Write to GIF' node specializes in creating and editing GIF animations from images. It can generate new GIFs from single images, append images to existing GIFs with transition effects, and adjust animation parameters such as frame duration and looping behavior. This node is designed to enhance visual content by enabling dynamic image transitions and preserving the continuity of animations.
    - Inputs:
        - `image` (Required): The image to be written into a GIF. This can be a new image for creating a GIF or an additional frame to be appended to an existing GIF animation. It plays a crucial role in determining the visual content of the GIF. Type should be `IMAGE`.
        - `transition_frames` (Required): Specifies the number of frames to be used for transitions between images in the GIF, affecting the smoothness and duration of the animation. Type should be `INT`.
        - `image_delay_ms` (Required): The delay in milliseconds before transitioning to the next image, influencing the pacing of the GIF animation. Type should be `FLOAT`.
        - `duration_ms` (Required): The duration in milliseconds for each frame in the GIF, determining how long each image is displayed. Type should be `FLOAT`.
        - `loops` (Required): The number of times the GIF animation will loop, with 0 indicating infinite looping. This affects the replayability of the GIF. Type should be `INT`.
        - `max_size` (Required): The maximum size of the images in the GIF, ensuring that the GIF does not exceed a certain dimension for compatibility and performance reasons. Type should be `INT`.
        - `output_path` (Required): The directory path where the GIF is to be saved. It specifies the location where the output animation is stored. Type should be `STRING`.
        - `filename` (Required): The name of the file for the output GIF, determining the filename under which the GIF will be saved. Type should be `STRING`.
    - Outputs:
        - `image_pass`: The original image or the last frame added to the GIF, indicating the final visual state of the GIF animation. Type should be `IMAGE`.
        - `filepath_text`: The full file path of the saved or edited GIF, providing a reference to the location of the GIF file. Type should be `STRING`.
        - `filename_text`: The name of the GIF file, offering a simple identifier for the generated or modified GIF animation. Type should be `STRING`.