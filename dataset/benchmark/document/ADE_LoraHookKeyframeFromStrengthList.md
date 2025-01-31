- `ADE_LoraHookKeyframeFromStrengthList`: This node is designed to create a sequence of LoRA hook keyframes based on a list of strengths, facilitating the dynamic adjustment of model behavior over a series of steps. It allows for the customization of keyframe properties such as strength and start percentage, enabling precise control over the animation or transformation process.
    - Inputs:
        - `strengths_float` (Required): Specifies the strengths for each keyframe in the sequence. This parameter can accept either a single float value or a list of float values, allowing for flexibility in defining the intensity of each keyframe. Type should be `FLOAT`.
        - `start_percent` (Required): Defines the starting percentage for the keyframe sequence, setting the initial point of the animation or transformation. Type should be `FLOAT`.
        - `end_percent` (Required): Sets the ending percentage for the keyframe sequence, marking the final point of the animation or transformation. Type should be `FLOAT`.
        - `print_keyframes` (Required): A boolean flag that, when enabled, prints the details of each keyframe to the log, aiding in debugging and visualization of the keyframe sequence. Type should be `BOOLEAN`.
        - `prev_hook_kf` (Optional): An optional parameter that allows for the continuation from a previous sequence of LoRA hook keyframes, enabling seamless transitions between sequences. Type should be `LORA_HOOK_KEYFRAMES`.
    - Outputs:
        - `HOOK_KF`: Returns a group of LoRA hook keyframes, representing the sequence of adjustments to be applied to the model. Type should be `LORA_HOOK_KEYFRAMES`.
