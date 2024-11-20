- `ADE_AdjustPESweetspotStretch`: This node is designed to adjust the position encoding (PE) sweetspot stretch in the AnimateDiff framework, allowing for dynamic modification of the PE stretch based on input parameters. It facilitates the fine-tuning of animation effects by modifying how the position encoding adapts over the course of an animation.
    - Inputs:
        - `sweetspot` (Required): Defines the initial position encoding length, serving as a baseline for adjustments. Type should be `INT`.
        - `new_sweetspot` (Required): Specifies the target position encoding length to adjust towards, enabling the stretch or compression of the encoding. Type should be `INT`.
        - `print_adjustment` (Required): A flag to control the logging of adjustment details, aiding in debugging and fine-tuning. Type should be `BOOLEAN`.
        - `prev_pe_adjust` (Optional): Allows for the incorporation of previous position encoding adjustments, enabling cumulative modifications. Type should be `PE_ADJUST`.
    - Outputs:
        - `pe_adjust`: Returns the updated position encoding adjustment, encapsulating the modifications applied. Type should be `PE_ADJUST`.