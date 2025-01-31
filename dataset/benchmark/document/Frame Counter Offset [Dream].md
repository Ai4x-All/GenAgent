- `Frame Counter Offset [Dream]`: The Frame Counter Offset node is designed to modify the frame counter by applying a specified offset value. This adjustment allows for the dynamic alteration of animation timelines, enabling the creation of shifted or delayed animation sequences based on the original frame count.
    - Inputs:
        - `frame_counter` (Required): The frame counter input represents the current state of an animation's frame count, including information such as the current frame, total frames, and frames per second. The offset applied to this counter can shift the animation timeline forward or backward. Type should be `FRAME_COUNTER`.
        - `offset` (Required): The offset parameter specifies the number of frames by which the frame counter should be incremented or decremented. This allows for the adjustment of the animation's timeline, effectively shifting the sequence of frames. Type should be `INT`.
    - Outputs:
        - `frame_counter`: The modified frame counter, which has been incremented or decremented by the specified offset, reflecting the new position in the animation timeline. Type should be `FRAME_COUNTER`.
