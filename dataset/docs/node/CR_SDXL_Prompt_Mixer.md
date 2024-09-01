- `CR SDXL Prompt Mixer`: The CR SDXL Prompt Mixer node is designed to blend and manipulate text prompts and styles for generative models, allowing for the creation of customized prompt combinations based on user-defined positive and negative prompts and styles, as well as preset configurations. This node facilitates the exploration of creative prompt variations to influence the generative process.
    - Parameters:
        - `prompt_positive`: The positive prompt text that contributes to the desired attributes or themes in the generated content. Type should be `STRING`.
        - `prompt_negative`: The negative prompt text that specifies undesired attributes or themes to be minimized or avoided in the generated content. Type should be `STRING`.
        - `style_positive`: The positive style text that defines the desired stylistic attributes to be emphasized in the generated content. Type should be `STRING`.
        - `style_negative`: The negative style text that specifies undesired stylistic attributes to be minimized or avoided in the generated content. Type should be `STRING`.
        - `preset`: A predefined configuration that determines how the positive and negative prompts and styles are mixed and applied. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `pos_g`: The global positive prompt text after mixing based on the selected preset. Type should be `STRING`.
        - `pos_l`: The local positive prompt text after mixing based on the selected preset. Type should be `STRING`.
        - `pos_r`: The right-aligned positive prompt text after mixing based on the selected preset. Type should be `STRING`.
        - `neg_g`: The global negative prompt text after mixing based on the selected preset. Type should be `STRING`.
        - `neg_l`: The local negative prompt text after mixing based on the selected preset. Type should be `STRING`.
        - `neg_r`: The right-aligned negative prompt text after mixing based on the selected preset. Type should be `STRING`.