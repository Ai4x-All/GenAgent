- `SaltLoadFileByIndexOrName`: This node is designed to load a file's content based on either its index within a directory or its name. It streamlines the process of retrieving file data, making it accessible for further processing or analysis.
    - Inputs:
        - `path` (Required): Specifies the path to the directory containing the file to be loaded. It is crucial for locating the target file within the filesystem. Type should be `STRING`.
        - `file_identifier` (Required): Acts as a unique identifier for the file to be loaded, which can be either the file's name or its index within the specified directory. This flexibility allows for easy reference to files without needing to know their exact names. Type should be `STRING`.
    - Outputs:
        - `file_content`: The content of the loaded file, returned as a string. This output makes the file's data readily available for use in subsequent operations. Type should be `STRING`.
