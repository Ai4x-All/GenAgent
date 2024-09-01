- `SaltKeyframeScheduler`: The SaltKeyframeScheduler node is designed for generating and manipulating keyframe schedules based on specified easing functions and custom parameters. It allows for the dynamic creation of animation or effect timelines by applying easing modes to keyframe sequences, enabling precise control over the timing and progression of visual or auditory effects.
    - Parameters:
        - `keyframe_schedule`: Defines the sequence of keyframes to be scheduled. This sequence forms the basis of the animation or effect timeline, dictating the key points of transition or change. Type should be `STRING`.
        - `easing_mode`: Specifies the easing function to apply to the keyframe schedule, influencing the interpolation and transition between keyframes. Type should be `COMBO[STRING]`.
        - `end_frame`: Determines the last frame of the schedule to consider for processing, allowing for partial scheduling within a larger sequence. Type should be `INT`.
        - `ndigits`: Sets the precision of the computed schedule values, defining how many decimal places to include. Type should be `INT`.
    - Inputs:
        - `a`: Custom parameter 'a' for additional flexibility in defining the scheduling logic or easing function behavior. Type should be `*`.
        - `b`: Custom parameter 'b', similar to 'a', for further customization of the scheduling or easing function. Type should be `*`.
    - Outputs:
        - `schedule_list`: The resulting list of scheduled keyframe values after applying the specified easing mode and custom parameters. Type should be `LIST`.