- `ADE_AnimateDiffModelSettingsSimple`: This node is designed to configure motion model settings for simple scenarios within the AnimateDiff framework. It allows for the adjustment of motion scale parameters and the application of optional masks to fine-tune the animation process.
    - Parameters:
        - `motion_pe_stretch`: Defines the stretch factor of positional encoding in the motion model, affecting the scale and intensity of motion applied. Type should be `INT`.
        - `min_motion_scale`: Sets the minimum scale for motion, providing a baseline for motion intensity. Type should be `FLOAT`.
        - `max_motion_scale`: Determines the maximum scale for motion, capping the intensity of motion effects. Type should be `FLOAT`.
    - Inputs:
        - `mask_motion_scale`: An optional mask tensor to apply scaling selectively across different regions, enhancing control over motion effects. Type should be `MASK`.
    - Outputs:
        - `ad_settings`: Outputs the configured motion model settings, encapsulating adjustments made to motion scale and optional masking. Type should be `AD_SETTINGS`.