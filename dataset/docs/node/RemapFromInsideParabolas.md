- `RemapFromInsideParabolas`: This node is designed to perform a remapping operation from the perspective of inside two parabolas, transforming an image based on specified parabolic contours and dimensions. It utilizes geometric transformations to adjust the image's representation, aligning it with the curvature and orientation defined by the parabolas.
    - Parameters:
        - `width`: Defines the width of the output image after remapping. This parameter allows for adjusting the scale of the transformed image. Type should be `INT`.
        - `height`: Specifies the height of the output image after remapping, enabling control over the vertical scale of the transformed image. Type should be `INT`.
    - Inputs:
        - `src_mask_with_i_parabolas`: Specifies the source mask that contains two parabolas, which are used to define the transformation geometry. This mask is crucial for determining how the image will be remapped according to the parabolic contours. Type should be `MASK`.
    - Outputs:
        - `remap`: The result of the remapping operation, which is an image transformed to align with the specified parabolic contours and dimensions. Type should be `REMAP`.