- `PromptComposerEffect`: The PromptComposerEffect node is designed to apply a specified effect with a given weight to an input text, enhancing the prompt composition process by allowing for dynamic customization based on the effect's intensity.
    - Parameters:
        - `effect`: Specifies the effect to be applied to the input text. This parameter determines the nature of the modification. Type should be `COMBO[STRING]`.
        - `effect_weight`: Defines the intensity of the applied effect, allowing for fine-tuned control over the modification's impact. Type should be `FLOAT`.
        - `active`: A boolean parameter that activates or deactivates the effect application, providing a way to enable or disable the effect dynamically. Type should be `BOOLEAN`.
        - `text_in_opt`: An optional input text to which an effect can be applied. It serves as the base text for further modification. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `text_out`: The output text with the specified effect applied, reflecting the modifications based on the effect's weight and activation status. Type should be `STRING`.