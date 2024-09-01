- `BitwiseAndMaskForEach`: This node is designed to perform a bitwise AND operation on each mask within a collection, effectively combining multiple masks into a single mask that represents the intersection of all input masks. It's aimed at processing scenarios where the overlap between various masks needs to be identified and isolated, making it suitable for applications requiring precise mask manipulation and analysis.
    - Parameters:
    - Inputs:
        - `base_segs`: The first mask to be combined using a bitwise AND operation. It plays a crucial role in determining the final output by intersecting its content with the second mask, thus affecting the node's execution and results. Type should be `SEGS`.
        - `mask_segs`: The second mask to be combined with the first mask using a bitwise AND operation. This mask contributes equally to the final output by intersecting with the first mask, influencing the node's execution and the characteristics of the resulting mask. Type should be `SEGS`.
    - Outputs:
        - `segs`: The resulting mask after performing the bitwise AND operation on the input masks. It represents the intersection of the input masks, highlighting areas where both masks overlap. Type should be `SEGS`.