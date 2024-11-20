- `LoadJsonFromUrl`: The node is designed to fetch JSON data from a specified URL, providing a straightforward way to load and integrate external data into the node's workflow.
    - Inputs:
        - `url` (Required): The URL from which JSON data is to be fetched. It serves as the primary source for the node to retrieve data. Type should be `STRING`.
        - `print_to_console` (Optional): A flag to control whether the fetched JSON content should be printed to the console, aiding in debugging or verification. Type should be `BOOLEAN`.
    - Outputs:
        - `json`: The JSON data retrieved from the specified URL, ready for further processing or utilization within the node's workflow. Type should be `JSON`.