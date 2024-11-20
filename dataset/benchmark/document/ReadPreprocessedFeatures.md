- `ReadPreprocessedFeatures`: This node is designed to read preprocessed feature data from a specified file path, loading it into a numpy array format for further processing or analysis.
    - Inputs:
        - `file_path` (Required): Specifies the path to the file containing the preprocessed features. This path is essential for locating and loading the data correctly. Type should be `STRING`.
    - Outputs:
        - `features`: Outputs the preprocessed features loaded from the file as a numpy array, ready for use in subsequent processing steps. Type should be `NP_ARRAY`.