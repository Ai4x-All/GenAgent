- `ThemeStylerAdvanced`: The ThemeStylerAdvanced node dynamically applies thematic styling to text prompts based on a selection of predefined themes. It enhances the original text by incorporating stylistic elements related to the chosen theme, aiming to modify the tone, mood, or visual imagery suggested by the text.
    - Inputs:
        - `text_positive_g` (Required): The global positive text prompt to be styled, representing broad thematic content to be enhanced. Type should be `STRING`.
        - `text_positive_l` (Required): The local positive text prompt to be styled, focusing on specific details or elements to be emphasized within the theme. Type should be `STRING`.
        - `text_negative` (Required): The negative text prompt to be styled, indicating content or themes to be avoided or contrasted against the desired styling. Type should be `STRING`.
        - `theme` (Required): The selected theme for styling, determining the stylistic elements to be applied to the text prompts. Type should be `COMBO[STRING]`.
        - `negative_prompt_to` (Required): Specifies the scope of negative styling, whether to apply it globally, locally, or both. Type should be `COMBO[STRING]`.
        - `log_prompt` (Required): A boolean flag to enable or disable logging of the prompt transformation process, providing insight into the styling effects. Type should be `BOOLEAN`.
    - Outputs:
        - `text_positive_g`: The styled global positive text prompt, reflecting the overarching theme. Type should be `STRING`.
        - `text_positive_l`: The styled local positive text prompt, showcasing specific thematic enhancements. Type should be `STRING`.
        - `text_positive`: The combined styled positive text prompt, integrating both global and local thematic elements. Type should be `STRING`.
        - `text_negative_g`: The styled global negative text prompt, indicating broader content or themes that have been avoided or contrasted. Type should be `STRING`.
        - `text_negative_l`: The styled local negative text prompt, reflecting specific details or elements that have been contrasted against the theme. Type should be `STRING`.
        - `text_negative`: The combined styled negative text prompt, integrating both global and local contrasts to the desired theme. Type should be `STRING`.
