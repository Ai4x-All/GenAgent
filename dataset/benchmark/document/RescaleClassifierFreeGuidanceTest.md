- `RescaleClassifierFreeGuidanceTest`: This node applies a custom patch to a given model, modifying its classifier-free guidance sampling function. The patch rescales the guidance scale factor dynamically based on the standard deviation of the conditional and unconditional inputs, aiming to maintain a consistent scale of features across different guidance strengths.
    - Inputs:
        - `model` (Required): The model to which the patch will be applied. This patch modifies the model's classifier-free guidance sampling function to dynamically adjust the guidance scale. Type should be `MODEL`.
        - `multiplier` (Required): A scaling factor that blends the original and rescaled guidance signals, controlling the strength of the rescaling effect on the model's output. Type should be `FLOAT`.
    - Outputs:
        - `model`: The patched model with an updated classifier-free guidance sampling function that incorporates dynamic rescaling based on input standard deviations. Type should be `MODEL`.
