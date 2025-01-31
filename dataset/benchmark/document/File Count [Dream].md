- `File Count [Dream]`: This node counts the number of files in a specified directory that match given patterns, such as file extensions. It's designed to facilitate file management and organization tasks by providing a quick way to quantify relevant files within a project or dataset.
    - Inputs:
        - `directory_path` (Required): Specifies the path to the directory where files will be counted. This path is essential for the node to locate and assess the files present in the desired location. Type should be `STRING`.
        - `patterns` (Required): Defines the file patterns (e.g., '*.jpg', '*.png') to match against files in the directory. This allows for filtering and counting files of specific types, enhancing the node's utility in managing and organizing files. Type should be `STRING`.
    - Outputs:
        - `TOTAL`: The total count of files matching the specified patterns within the given directory. This output provides a straightforward metric for assessing the volume of relevant files. Type should be `INT`.
