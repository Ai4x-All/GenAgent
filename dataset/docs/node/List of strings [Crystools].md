- `List of strings [Crystools]`: This node is designed to aggregate multiple string inputs into a single list or a concatenated string, based on the provided delimiter. It facilitates the handling and manipulation of string collections within the Crystools framework, emphasizing ease of string data aggregation and manipulation.
    - Parameters:
        - `string_i`: Represents one of the eight possible string inputs for aggregation. Each contributes to the formation of the list or the concatenated string output, depending on the presence of a delimiter. Type should be `STRING`.
        - `delimiter`: A delimiter string used to concatenate the provided string inputs into a single string, if specified. Its presence or absence determines the output format (list or concatenated string). Type should be `STRING`.
    - Inputs:
    - Outputs:
        - `concatenated`: The concatenated string result of aggregating the input strings with the specified delimiter. Type should be `STRING`.
        - `list_string`: A list containing the input strings, showcasing the node's ability to aggregate string data into a structured collection. Type should be `ListString`.