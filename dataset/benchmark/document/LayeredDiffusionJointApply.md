- `LayeredDiffusionJointApply`: This node applies a joint layered diffusion process to generate or modify images, leveraging a combination of conditional and unconditional inputs to enhance the quality and relevance of the output. It integrates multiple diffusion models to process and blend latent representations, facilitating nuanced image synthesis or transformation.
    - Inputs:
        - `model` (Required): The model patcher that configures and applies the diffusion models, acting as the intermediary for executing the layered diffusion process. Type should be `MODEL`.
        - `config` (Required): Configuration string that specifies the particular diffusion model to be used, ensuring compatibility and optimal performance. Type should be `COMBO[STRING]`.
        - `fg_cond` (Optional): Foreground conditional inputs that guide the diffusion process towards generating images with specific foreground characteristics. Type should be `CONDITIONING`.
        - `bg_cond` (Optional): Background conditional inputs that influence the diffusion process to generate images with specific background characteristics. Type should be `CONDITIONING`.
        - `blended_cond` (Optional): Blended conditional inputs that combine foreground and background characteristics, enriching the diffusion process. Type should be `CONDITIONING`.
    - Outputs:
        - `model`: The modified model after applying the layered diffusion process, ready for further image generation or transformation tasks. Type should be `MODEL`.