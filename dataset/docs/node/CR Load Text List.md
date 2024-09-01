- `CR Load Text List`: This node is designed to load and parse text lists from files with specific extensions, such as .txt or .csv, facilitating the handling and manipulation of textual data within a workflow.
    - Parameters:
        - `input_file_path`: Specifies the path to the directory containing the target file, playing a crucial role in locating the file for data extraction. Type should be `STRING`.
        - `file_name`: The name of the file (excluding its extension) to be loaded. This parameter is essential for identifying the specific file to be processed. Type should be `STRING`.
        - `file_extension`: Defines the file extension (e.g., 'txt', 'csv') of the target file, determining the method of parsing and loading the text list. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `STRING`: Returns a list of strings extracted from the specified file. Type should be `STRING`.
        - `show_help`: Provides a URL offering additional help and guidance on using the node. Type should be `STRING`.