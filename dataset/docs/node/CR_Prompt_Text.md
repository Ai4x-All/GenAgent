- `CR Prompt Text`: This node is designed to process and return a user-defined text prompt, along with a help URL for further guidance. It primarily serves as a utility for text input handling within a broader system, facilitating user interaction by accepting and returning text prompts.
    - Parameters:
        - `prompt`: The 'prompt' parameter is the user-defined text input that the node processes. It plays a crucial role in the node's operation by being the main piece of information that gets returned along with a help URL. Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `prompt`: The 'prompt' output is the user-defined text input that was processed by the node. Type should be `STRING`.
        - `show_help`: The 'show_help' output provides a URL to a help page, offering users additional information and guidance on using the node. Type should be `STRING`.