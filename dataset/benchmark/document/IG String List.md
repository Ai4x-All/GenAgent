- `IG String List`: The IG String List node is designed to split a multiline string input into a list of strings based on newline characters and return a specific string from the list and the entire list itself. It allows for dynamic text manipulation and retrieval within a user-defined list, facilitating operations on collections of strings.
    - Inputs:
        - `index` (Required): Specifies the position in the list of strings to retrieve the specific string. It determines which string to return based on its position in the list, enhancing the node's flexibility in accessing elements. Type should be `INT`.
        - `string_list` (Required): A multiline string input that the node splits into a list of strings based on newline characters. This input is essential for creating the string list that the node operates on, enabling dynamic text manipulation. Type should be `STRING`.
    - Outputs:
        - `current value`: Returns the string at the specified index from the list of strings, allowing for targeted retrieval of text. Type should be `STRING`.
        - `list`: Returns the entire list of strings derived from the input multiline string, providing access to all split text elements. Type should be `STRING`.