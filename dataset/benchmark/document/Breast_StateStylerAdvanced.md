- `Breast_StateStylerAdvanced`: The Breast_StateStylerAdvanced node is designed to apply advanced styling options to text prompts, leveraging a comprehensive set of styling parameters to enhance or modify the aesthetic and thematic elements of the input text. It abstracts complex styling operations into a user-friendly interface, allowing for detailed customization and refinement of text-based content.
    - Inputs:
        - `text_positive_g` (Required): Represents the global positive text prompt for styling, setting the broad thematic direction. Type should be `STRING`.
        - `text_positive_l` (Required): Specifies the local positive text prompt, allowing for finer thematic adjustments within the global context. Type should be `STRING`.
        - `text_negative` (Required): The initial negative text prompt that the node will modify to counterbalance or avoid specific themes. Type should be `STRING`.
        - `breast_state` (Required): unknown Type should be `COMBO[STRING]`.
        - `negative_prompt_to` (Required): Determines how the negative styling is applied, offering options to target global, local, or both aspects of the text. Type should be `COMBO[STRING]`.
        - `log_prompt` (Required): A boolean flag that enables logging of the styling process, providing insights into the selections made and the transformations applied. Type should be `BOOLEAN`.
    - Outputs:
        - `text_positive_g`: The styled global positive text prompt, reflecting broad thematic enhancements. Type should be `STRING`.
        - `text_positive_l`: The styled local positive text prompt, showcasing finer adjustments within the global theme. Type should be `STRING`.
        - `text_positive`: A composite of the global and local positive prompts, fully styled. Type should be `STRING`.
        - `text_negative_g`: The styled global negative text prompt, modified to counterbalance or avoid specific global themes. Type should be `STRING`.
        - `text_negative_l`: The styled local negative text prompt, addressing finer thematic elements to be avoided or counterbalanced. Type should be `STRING`.
        - `text_negative`: A composite of the global and local negative prompts, fully styled to avoid or counterbalance specific themes. Type should be `STRING`.
