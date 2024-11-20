- `RegionalPrompt`: The RegionalPrompt node is designed to generate regional prompts based on specified masks and advanced samplers. It allows for the creation of customized prompts that can be applied to specific regions of an image, enabling targeted modifications or enhancements. This functionality is particularly useful in scenarios where different areas of an image require distinct treatments or effects, facilitating a more granular control over the generation process.
    - Inputs:
        - `mask` (Required): Specifies the region mask to apply the prompt to, defining the area of the image that will be affected by the generated prompt. Type should be `MASK`.
        - `advanced_sampler` (Required): Determines the advanced sampling technique to be used for the specified region, influencing how the prompt is applied and the resulting modifications. Type should be `KSAMPLER_ADVANCED`.
        - `variation_seed` (Optional): Controls the seed for variations in the prompt generation, allowing for reproducibility or diversity in the outputs. Type should be `INT`.
        - `variation_strength` (Optional): Adjusts the strength of variations applied to the prompt, enabling fine-tuning of the prompt's impact on the region. Type should be `FLOAT`.
        - `variation_method` (Optional): Selects the method for applying variations to the prompt, such as linear or spherical linear interpolation (slerp), affecting the nature of the prompt modifications. Type should be `COMBO[STRING]`.
    - Outputs:
        - `regional_prompts`: Generates regional prompts that can be utilized in the RegionalSampler, tailored to the specified regions with the applied variations. Type should be `REGIONAL_PROMPTS`.