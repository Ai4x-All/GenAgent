- `Inference_Core_LayeredDiffusionCondJointApply`: This node specializes in applying conditional and joint layered diffusion processes to generate or manipulate images based on a set of conditions and joint configurations. It integrates multiple diffusion models to achieve complex image synthesis or transformation tasks, leveraging conditional inputs and joint model dynamics.
    - Inputs:
        - `model` (Required): The model patcher used to apply layered diffusion techniques, essential for integrating with the diffusion process. Type should be `MODEL`.
        - `image` (Required): The target image for the diffusion process, serving as a basis for transformations or synthesis. Type should be `IMAGE`.
        - `config` (Required): A configuration string that determines the specific layered diffusion model and settings to use. Type should be `COMBO[STRING]`.
        - `cond` (Optional): Optional conditional inputs for the diffusion process, allowing for targeted image manipulation or generation. Type should be `CONDITIONING`.
        - `blended_cond` (Optional): Optional blended conditional inputs, enabling more complex image synthesis by combining conditions. Type should be `CONDITIONING`.
    - Outputs:
        - `model`: Outputs the model after applying the layered diffusion process, equipped with modifications for image synthesis or transformation. Type should be `MODEL`.