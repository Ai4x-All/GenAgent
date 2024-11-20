- `ImpactStringSelector`: The ImpactStringSelector node is designed to select a specific string or a set of strings from a given multiline string input based on user-defined criteria. It allows for the extraction of meaningful data or segments from larger text blocks, facilitating text manipulation and processing tasks within a workflow.
    - Inputs:
        - `strings` (Required): A multiline string from which specific strings or segments are to be selected. This parameter is crucial for defining the source text for selection. Type should be `STRING`.
        - `multiline` (Required): A boolean flag indicating whether the selection should consider each line as a separate entity or treat the entire input as a single string. This affects how the selection is made. Type should be `BOOLEAN`.
        - `select` (Required): An integer specifying the index of the string or line to be selected from the input. This determines which part of the input is extracted and returned. Type should be `INT`.
    - Outputs:
        - `string`: The selected string or line based on the specified index and criteria. This output is the result of the selection process. Type should be `STRING`.