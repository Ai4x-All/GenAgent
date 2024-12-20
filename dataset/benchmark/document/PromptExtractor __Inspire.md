- `PromptExtractor __Inspire`: The PromptExtractor node in the Inspire pack is designed to extract and process prompt information from images, facilitating the customization and manipulation of prompts based on specific inputs. It serves as a bridge between the visual content and the textual prompt generation process, enabling dynamic prompt creation and modification.
    - Inputs:
        - `image` (Required): The 'image' input type is used to provide the visual content from which prompts will be extracted or based upon. Type should be `COMBO[STRING]`.
        - `positive_id` (Required): The 'positive_id' input specifies the identifier for selecting the positive prompt text from the available options. Type should be `STRING`.
        - `negative_id` (Required): The 'negative_id' input specifies the identifier for selecting the negative prompt text from the available options. Type should be `STRING`.
        - `info` (Required): The 'info' input type is used for providing additional information or context that may influence the prompt extraction process. Type should be `STRING`.
    - Outputs:
        - `positive`: This output type represents the extracted positive prompt text. Type should be `STRING`.
        - `negative`: This output type represents the extracted negative prompt text. Type should be `STRING`.
