- `LayerUtility_ PromptTagger`: The PromptTagger node is designed to enhance and modify text prompts based on specific criteria such as token limits and exclusion or replacement of words. It primarily serves to prepare and optimize prompts for further processing or generation tasks, ensuring they meet the required specifications for use with certain APIs or models.
    - Inputs:
        - `image` (Required): The image input is used as a reference for generating or modifying the text prompt, providing visual context that influences the output. Type should be `IMAGE`.
        - `api` (Required): Specifies the API to be used, with 'gemini-pro-vision' being a supported option. This determines the processing or generation capabilities available for the prompt. Type should be `COMBO[STRING]`.
        - `token_limit` (Required): Defines the maximum number of tokens allowed in the prompt, ensuring it adheres to specific API or model constraints. Type should be `INT`.
        - `exclude_word` (Required): A word to be excluded from the prompt, allowing for customization and refinement of the generated text. Type should be `STRING`.
        - `replace_with_word` (Required): Specifies a word to replace within the prompt, enabling targeted modifications to the text. Type should be `STRING`.
    - Outputs:
        - `text`: The modified or enhanced text prompt, ready for further processing or use. Type should be `STRING`.