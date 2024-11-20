- `ControlNetHadamard`: This node applies a control network to a set of images and conditions, modulating the latter based on the control network's output and a specified strength. It's designed to integrate control network effects into image conditioning, allowing for dynamic adjustments to the conditioning process.
    - Inputs:
        - `conds` (Required): The conditions to be modulated by the control network, representing the contextual or semantic guidance for image generation. Type should be `CONDITIONING`.
        - `control_net` (Required): The control network to be applied, determining the nature and extent of modulation on the conditions. Type should be `CONTROL_NET`.
        - `image` (Required): The images to which the control network adjustments are applied, serving as the basis for condition modulation. Type should be `IMAGE`.
        - `strength` (Required): A scalar value determining the intensity of the control network's effect on the conditions, allowing for fine-tuned control over the modulation. Type should be `FLOAT`.
    - Outputs:
        - `conditioning`: The modulated conditions, adjusted by the control network to reflect the desired changes. Type should be `CONDITIONING`.