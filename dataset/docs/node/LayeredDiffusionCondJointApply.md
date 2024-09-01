- `LayeredDiffusionCondJointApply`: This node specializes in applying conditional and joint layered diffusion processes to generate or modify images based on specific conditions and joint configurations. It leverages advanced diffusion techniques to blend and refine images, ensuring high-quality outputs tailored to the given conditions.
    - Parameters:
        - `config`: Configuration string specifying the layered diffusion model to use, critical for selecting the appropriate processing approach. Type should be `COMBO[STRING]`.
    - Inputs:
        - `model`: The model patcher used to apply the layered diffusion process, crucial for adapting the base model to specific configurations and conditions. Type should be `MODEL`.
        - `image`: The image to be processed, serving as a base for the diffusion effects and transformations. Type should be `IMAGE`.
        - `cond`: The conditional inputs guiding the diffusion process, essential for tailoring the output to specific requirements or contexts. Type should be `CONDITIONING`.
        - `blended_cond`: Blended conditional inputs, combining multiple conditions to enrich the diffusion process and enhance output quality. Type should be `CONDITIONING`.
    - Outputs:
        - `model`: The modified model after applying the layered diffusion process, reflecting the changes and enhancements made. Type should be `MODEL`.