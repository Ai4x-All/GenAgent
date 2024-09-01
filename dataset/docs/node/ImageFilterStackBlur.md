- `ImageFilterStackBlur`: The ImageFilterStackBlur node applies a stack blur effect to images, a technique that simulates a bokeh-like blur by blending pixels in a specific radius around each point, resulting in a smooth and uniform effect.
    - Parameters:
        - `size_x`: Specifies the horizontal size of the blur effect. It influences the width of the area around each pixel that is considered for the blur. Type should be `INT`.
        - `size_y`: Specifies the vertical size of the blur effect. It influences the height of the area around each pixel that is considered for the blur. Type should be `INT`.
    - Inputs:
        - `images`: The images to apply the stack blur effect on. This is the primary input that determines the visual output of the node. Type should be `IMAGE`.
    - Outputs:
        - `image`: The resulting image after applying the stack blur effect, showcasing a smooth and visually appealing blur. Type should be `IMAGE`.