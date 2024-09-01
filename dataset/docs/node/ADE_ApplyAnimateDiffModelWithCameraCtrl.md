- `ADE_ApplyAnimateDiffModelWithCameraCtrl`: This node applies the AnimateDiff model with camera control, integrating motion model adjustments and camera control parameters to generate animated sequences. It leverages camera control poses and other animation parameters to enhance the AnimateDiff model's output, providing a more dynamic and customizable animation experience.
    - Parameters:
        - `start_percent`: The starting point of the animation as a percentage of the total animation length, allowing for partial animations. Type should be `FLOAT`.
        - `end_percent`: The ending point of the animation as a percentage of the total animation length, enabling customization of the animation's duration. Type should be `FLOAT`.
    - Inputs:
        - `motion_model`: The motion model to be animated, incorporating both the AnimateDiff model's capabilities and camera control features for enhanced animation. Type should be `MOTION_MODEL_ADE`.
        - `cameractrl_poses`: A list of camera control poses, each defining a specific camera position and orientation to be applied during the animation process. Type should be `CAMERACTRL_POSES`.
        - `motion_lora`: Optional parameter for specifying motion LoRA settings to further customize the animation. Type should be `MOTION_LORA`.
        - `scale_multival`: Optional parameter for applying scale multipliers to the animation, affecting the overall size of animated elements. Type should be `MULTIVAL`.
        - `effect_multival`: Optional parameter for applying effect multipliers, allowing for additional visual effects in the animation. Type should be `MULTIVAL`.
        - `cameractrl_multival`: Optional parameter for applying multiple camera control values, enhancing the dynamic camera movements within the animation. Type should be `MULTIVAL`.
        - `ad_keyframes`: Optional parameter for defining keyframes within the animation, enabling precise control over animation sequences. Type should be `AD_KEYFRAMES`.
        - `prev_m_models`: Optional parameter for incorporating previously generated motion models, facilitating sequential or layered animations. Type should be `M_MODELS`.
    - Outputs:
        - `m_models`: The resulting motion models after applying the AnimateDiff model with camera control, including any specified animations and effects. Type should be `M_MODELS`.