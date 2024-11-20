- `ImageApplyLUT+`: This node applies a Look-Up Table (LUT) to an image or a batch of images to modify their appearance based on the LUT's defined transformations. It supports optional gamma correction, clipping of LUT values, and blending the transformed image with the original based on a specified strength. This process allows for sophisticated color grading and image effect applications.
    - Inputs:
        - `image` (Required): The image or batch of images to which the LUT will be applied. This is the primary input that undergoes transformation. Type should be `IMAGE`.
        - `lut_file` (Required): The filename of the Look-Up Table (LUT) to be applied. This determines the specific color transformation to be executed. Type should be `COMBO[STRING]`.
        - `gamma_correction` (Required): A boolean flag indicating whether gamma correction should be applied to the image before and after LUT application, enhancing the visual quality. Type should be `BOOLEAN`.
        - `clip_values` (Required): A boolean flag that, when true, clips the LUT values to ensure they stay within the defined domain, preventing potential color distortion. Type should be `BOOLEAN`.
        - `strength` (Required): A float value between 0 and 1 indicating the blend strength of the LUT-applied image with the original image, allowing for subtle to full application of the LUT effect. Type should be `FLOAT`.
    - Outputs:
        - `image`: The transformed image or batch of images after the LUT has been applied, optionally gamma-corrected and blended with the original based on the specified strength. Type should be `IMAGE`.