- `RescaleCFG`: The RescaleCFG node is designed to adjust the conditioning and unconditioning scales of a model's output based on a specified multiplier, aiming to achieve a more balanced and controlled generation process. It operates by rescaling the model's output to modify the influence of conditioned and unconditioned components, thereby potentially enhancing the model's performance or output quality.
    - Inputs:
        - `model` (Required): The model parameter represents the generative model to be adjusted. It is crucial as the node applies a rescaling function to the model's output, directly influencing the generation process. Type should be `MODEL`.
        - `multiplier` (Required): The multiplier parameter controls the extent of rescaling applied to the model's output. It determines the balance between the original and rescaled components, affecting the final output's characteristics. Type should be `FLOAT`.
    - Outputs:
        - `model`: The modified model with adjusted conditioning and unconditioning scales. This model is expected to produce outputs with potentially enhanced characteristics due to the applied rescaling. Type should be `MODEL`.
