- `CR Save Text To File`: The CR_SaveTextToFile node is designed for saving text data to a file, supporting both plain text and CSV formats. It intelligently handles file naming to avoid overwriting existing files and provides flexibility in specifying the output file's location, name, and extension.
    - Inputs:
        - `multiline_text` (Required): The text content to be saved, which can be in multiline format. This content is either saved as plain text or parsed into a CSV format based on the file extension provided. Type should be `STRING`.
        - `output_file_path` (Required): The directory path where the output file will be saved. It is part of the final filepath construction. Type should be `STRING`.
        - `file_name` (Required): The base name of the output file. If a file with the same name already exists, the node will append a numerical suffix to ensure uniqueness. Type should be `STRING`.
        - `file_extension` (Required): The extension of the output file, determining whether the content is saved as plain text or CSV format. Type should be `COMBO[STRING]`.
    - Outputs:
        - `show_help`: A URL to the node's documentation, providing additional help and examples. Type should be `STRING`.
