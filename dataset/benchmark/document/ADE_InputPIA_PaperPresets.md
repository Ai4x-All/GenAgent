- `ADE_InputPIA_PaperPresets`: This node is designed to generate input parameters for the AnimateDiff-PIA model based on predefined paper presets. It allows users to select a preset configuration, which is then used to configure the AnimateDiff-PIA model for animation generation, providing a simplified way to apply complex animation effects.
    - Inputs:
        - `preset` (Required): Specifies the preset configuration to use for the AnimateDiff-PIA model. Each preset corresponds to a predefined set of parameters that define specific animation effects. Type should be `COMBO[STRING]`.
        - `batch_index` (Required): Determines the index of the batch for which the input is being generated. This is used to manage multiple animation inputs within a batch processing context. Type should be `INT`.
        - `mult_multival` (Optional): An optional multiplier that can be applied to multiple values within the preset, allowing for further customization of the animation effect. Type should be `MULTIVAL`.
        - `print_values` (Optional): When set to True, the selected preset's parameters are logged, providing insight into the specific configuration being applied. Type should be `BOOLEAN`.
    - Outputs:
        - `pia_input`: Generates a configured input for the AnimateDiff-PIA model based on the selected paper preset. Type should be `PIA_INPUT`.