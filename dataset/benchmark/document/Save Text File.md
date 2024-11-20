- `Save Text File`: This node is designed to save a given text to a file, handling path and filename generation with customizable options. It ensures the creation of the specified path if it doesn't exist, validates the text content, and updates a history of saved text files.
    - Inputs:
        - `text` (Required): The text content to be saved. It's crucial as it determines the content of the created text file. Type should be `STRING`.
        - `path` (Required): The destination path where the text file will be saved. The node supports token parsing for dynamic path generation. Type should be `STRING`.
        - `filename_prefix` (Required): An optional prefix for the filename, supporting token parsing for dynamic generation. Type should be `STRING`.
        - `filename_delimiter` (Required): A delimiter used in the filename to separate different parts, such as the prefix from the generated number. Type should be `STRING`.
        - `filename_number_padding` (Required): Determines the padding for the numerical part of the filename, ensuring a consistent filename format. Type should be `INT`.
    - Outputs: