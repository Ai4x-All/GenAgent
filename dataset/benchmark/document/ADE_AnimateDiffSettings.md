- `ADE_AnimateDiffSettings`: This node is designed to configure settings for the animation difference process, allowing users to adjust parameters related to positional encoding and weight adjustments. It serves as a foundational element in customizing the behavior and output of animation difference operations.
    - Inputs:
        - `pe_adjust` (Optional): Specifies the adjustments to be made to the positional encoding, influencing how animation frames are generated and interpolated. Type should be `PE_ADJUST`.
        - `weight_adjust` (Optional): Defines the adjustments to the weights, affecting the influence of different components in the animation difference calculation. Type should be `WEIGHT_ADJUST`.
    - Outputs:
        - `ad_settings`: The configured animation difference settings, ready to be applied in subsequent animation difference processes. Type should be `AD_SETTINGS`.
