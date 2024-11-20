- `SDXLPromptStyler`: The SDXLPromptStyler node is designed to process and style text prompts based on specified styles and templates. It modifies the input positive and negative prompts by incorporating them into predefined templates, allowing for dynamic and context-aware text generation.
    - Inputs:
        - `text_positive` (Required): The positive text input that will be styled according to the specified template and style. It plays a crucial role in shaping the output's positive sentiment. Type should be `STRING`.
        - `text_negative` (Required): The negative text input that will be combined with the template's negative prompt, if present, to tailor the output's negative sentiment. Type should be `STRING`.
        - `style` (Required): Specifies the styling template to be applied to the text inputs, influencing the thematic presentation of the generated prompts. Type should be `COMBO[STRING]`.
        - `log_prompt` (Required): Controls whether the styling process details are logged, aiding in debugging and process transparency. Type should be `COMBO[STRING]`.
    - Outputs:
        - `text_positive`: The styled positive text, transformed according to the specified style and template. Type should be `STRING`.
        - `text_negative`: The styled negative text, adjusted to complement the positive text in accordance with the template's guidelines. Type should be `STRING`.