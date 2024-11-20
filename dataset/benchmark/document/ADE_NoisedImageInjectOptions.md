- `ADE_NoisedImageInjectOptions`: This node is designed to create and configure options for injecting noised images into an animation sequence. It allows for the specification of positional adjustments for the injected images, enabling precise control over their placement within the animation frames.
    - Inputs:
        - `composite_x` (Optional): Specifies the horizontal position offset for the image injection. This allows for fine-tuning the placement of the injected image within the frame. Type should be `INT`.
        - `composite_y` (Optional): Specifies the vertical position offset for the image injection. This enables precise vertical alignment of the injected image within the animation frame. Type should be `INT`.
    - Outputs:
        - `IMG_INJECT_OPTS`: Returns an instance of NoisedImageInjectOptions configured with the specified positional adjustments. This object is used to control the placement of noised images in the animation sequence. Type should be `IMAGE_INJECT_OPTIONS`.