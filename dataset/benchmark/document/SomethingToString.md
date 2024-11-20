- `SomethingToString`: This node is designed to convert various data types into a string format, optionally allowing for the addition of a prefix or suffix to the resulting string. It abstracts the complexity of data type conversion and string manipulation, providing a straightforward way to generate string representations of diverse inputs.
    - Inputs:
        - `input` (Required): The primary data that will be converted to a string. This input can be of any type, and its conversion is central to the node's functionality. Type should be `*`.
        - `prefix` (Optional): An optional string to prepend to the converted input, allowing for customization of the resulting string's format. Type should be `STRING`.
        - `suffix` (Optional): An optional string to append to the converted input, enhancing the flexibility in formatting the resulting string. Type should be `STRING`.
    - Outputs:
        - `string`: The output is the string representation of the input, potentially modified by the specified prefix and/or suffix. Type should be `STRING`.