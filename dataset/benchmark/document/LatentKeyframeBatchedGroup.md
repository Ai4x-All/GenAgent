- `LatentKeyframeBatchedGroup`: This node is designed to manage and manipulate batches of latent keyframes for advanced control in generative models. It allows for the creation, modification, and interpolation of keyframes based on specified strengths and batch indices, facilitating dynamic adjustments to the generative process.
    - Inputs:
        - `float_strengths` (Required): Defines the strengths for a batch of keyframes, enabling the creation or modification of multiple keyframes simultaneously. This parameter can accept either a single float value or an iterable of float values, allowing for flexible keyframe strength specification. Type should be `FLOAT`.
        - `prev_latent_kf` (Optional): An optional parameter that allows for the inclusion of previously defined latent keyframes, enabling their modification or extension with new keyframe data. Type should be `LATENT_KEYFRAME`.
        - `print_keyframes` (Optional): A flag that, when enabled, triggers logging of keyframe details for debugging or informational purposes. Type should be `BOOLEAN`.
        - `autosize` (Optional): An optional parameter that adjusts the size of the generated keyframes, providing flexibility in their presentation or storage. Type should be `ACNAUTOSIZE`.
    - Outputs:
        - `LATENT_KF`: The modified or newly created batch of latent keyframes, ready for use in further generative processes. Type should be `LATENT_KEYFRAME`.