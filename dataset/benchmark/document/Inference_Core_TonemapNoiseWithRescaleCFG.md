- `Inference_Core_TonemapNoiseWithRescaleCFG`: This node applies a tonemapping and noise rescaling configuration to a given model, enhancing its ability to handle conditional and unconditional inputs by adjusting their scale and contrast. It utilizes a combination of tonemapping techniques and rescaling factors to modify the model's sampling behavior, aiming to improve the quality and consistency of generated outputs.
    - Inputs:
        - `model` (Required): The model to which the tonemapping and noise rescaling configuration will be applied. This configuration adjusts the model's handling of inputs to enhance output quality. Type should be `MODEL`.
        - `tonemap_multiplier` (Required): A multiplier that adjusts the intensity of the tonemapping effect, influencing the contrast and brightness of the noise in the model's output. Type should be `FLOAT`.
        - `rescale_multiplier` (Required): A multiplier that adjusts the scale of the conditional generation, affecting the balance between the original and modified noise predictions in the final output. Type should be `FLOAT`.
    - Outputs:
        - `model`: The modified model with an updated sampling behavior, incorporating the specified tonemapping and noise rescaling configurations. Type should be `MODEL`.
