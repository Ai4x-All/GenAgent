- `ttN textDebug`: The ttN textDebug node is designed for debugging purposes within the tinyterra text processing framework. It allows for the inspection and manipulation of text data, providing a means to evaluate and refine text processing workflows.
    - Inputs:
        - `print_to_console` (Required): Determines whether the debugged text data should be printed to the console, facilitating real-time inspection. Type should be `COMBO[BOOLEAN]`.
        - `console_title` (Required): Specifies a title for the console output when 'print_to_console' is true, allowing for easier identification of the debugged text. Type should be `STRING`.
        - `execute` (Required): Controls when the node executes, with options like 'Always' or 'On Change', to optimize debugging efficiency. Type should be `COMBO[STRING]`.
        - `text` (Required): The 'text' input is essential for providing the text data to be debugged. It supports multiline input and dynamic prompts, enabling flexible and interactive debugging sessions. Type should be `STRING`.
    - Outputs:
        - `text`: The output 'text' is the processed or inspected text data, allowing for direct observation of the debugging results. Type should be `STRING`.