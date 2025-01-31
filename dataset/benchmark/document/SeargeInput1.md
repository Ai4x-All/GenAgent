- `SeargeInput1`: SeargeInput1 is designed to aggregate and organize various textual prompts and styles into a unified parameter set for further processing. It serves as a multiplexer, combining inputs related to main and secondary prompts, style descriptions, and negative prompts and styles, along with optional image and mask inputs, into a single, structured output.
    - Inputs:
        - `main_prompt` (Required): The primary text prompt for generating or influencing content. It serves as the main input for content creation or modification. Type should be `STRING`.
        - `secondary_prompt` (Required): A supplementary text prompt that provides additional context or direction alongside the main prompt. Type should be `STRING`.
        - `style_prompt` (Required): A text prompt that specifies the desired style or tone for the content being generated or modified. Type should be `STRING`.
        - `negative_prompt` (Required): A text prompt that indicates what themes or elements should be avoided in the generated content. Type should be `STRING`.
        - `negative_style` (Required): A text prompt that specifies styles or tones to be avoided in the content creation process. Type should be `STRING`.
        - `inputs` (Optional): An optional parameter for passing in previously defined inputs, allowing for dynamic input aggregation and modification. Type should be `PARAMETER_INPUTS`.
        - `image` (Optional): An optional image input that can be used to influence or guide the content generation process. Type should be `IMAGE`.
        - `mask` (Optional): An optional mask input for the image, used to specify areas of interest or exclusion in content generation. Type should be `MASK`.
    - Outputs:
        - `inputs`: The aggregated set of parameters, including prompts, styles, and optional image and mask inputs, structured for further processing. Type should be `PARAMETER_INPUTS`.
