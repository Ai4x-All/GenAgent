- `LivePortraitProcess`: The LivePortraitProcess node is designed to transform static portrait images into animated versions by applying a series of image processing and deep learning techniques. It leverages facial landmarks, cropping, resizing, and feature extraction to prepare the source image. Subsequently, it utilizes keypoints information, rotation matrices, and 3D features to animate the portrait based on driving images, adjusting for eye and lip movements, and optionally stitching the results for a seamless animation.
    - Inputs:
        - `pipeline` (Required): The processing pipeline that encapsulates the entire animation process, including cropping, feature extraction, and animation synthesis. Type should be `LIVEPORTRAITPIPE`.
        - `source_image` (Required): The source image to be animated. It serves as the base for the animation process, where facial features are detected and used to guide the transformation. Type should be `IMAGE`.
        - `driving_images` (Required): A sequence of images that dictate the animation's movements. These images provide the dynamic expressions and orientations to be transferred to the source portrait. Type should be `IMAGE`.
        - `dsize` (Required): The desired size for the output images, affecting how the source and driving images are cropped and resized. Type should be `INT`.
        - `scale` (Required): A scaling factor applied during the cropping process to adjust the emphasis on the central features of the portrait. Type should be `FLOAT`.
        - `vx_ratio` (Required): The horizontal ratio used to fine-tune the cropping area, focusing on the central facial features. Type should be `FLOAT`.
        - `vy_ratio` (Required): The vertical ratio used to fine-tune the cropping area, focusing on the central facial features. Type should be `FLOAT`.
        - `lip_zero` (Required): A flag indicating whether to neutralize lip movements in the animation, keeping the lips static. Type should be `BOOLEAN`.
        - `eye_retargeting` (Required): A flag to enable or disable eye movement retargeting in the animation, allowing for dynamic eye expressions. Type should be `BOOLEAN`.
        - `eyes_retargeting_multiplier` (Required): A multiplier applied to the eye movement retargeting, allowing for exaggerated or subdued eye animations. Type should be `FLOAT`.
        - `lip_retargeting` (Required): A flag to enable or disable lip movement retargeting in the animation, allowing for dynamic lip expressions. Type should be `BOOLEAN`.
        - `lip_retargeting_multiplier` (Required): A multiplier applied to the lip movement retargeting, allowing for exaggerated or subdued lip animations. Type should be `FLOAT`.
        - `stitching` (Required): A flag indicating whether to apply stitching to the animated frames, ensuring seamless transitions between expressions. Type should be `BOOLEAN`.
        - `relative` (Required): A flag that determines whether the animation should be based on relative movements from the driving images or absolute positions. Type should be `BOOLEAN`.
        - `onnx_device` (Optional): Specifies the computation device (e.g., CUDA for GPU) for running the ONNX models involved in the animation process. Type should be `COMBO[STRING]`.
    - Outputs:
        - `cropped_images`: A list of cropped and processed images ready for animation, representing intermediate steps in the animation pipeline. Type should be `IMAGE`.
        - `full_images`: The final list of animated portraits, fully processed and ready for display or further use. Type should be `IMAGE`.