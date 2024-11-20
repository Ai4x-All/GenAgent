- `SaltUpdateJSON`: The SaltUpdateJSON node is designed to update specific values within a JSON structure based on a given key. It recursively searches through the JSON, updating all instances of the key with a new value, thereby allowing for comprehensive modifications of nested JSON objects.
    - Inputs:
        - `json_input` (Required): The JSON string to be updated. It serves as the base structure for modifications, where specific values associated with a given key are targeted for updates. Type should be `STRING`.
        - `key` (Required): The key whose associated values are to be updated across the JSON structure. It acts as the identifier for locating and modifying specific data points within the JSON. Type should be `STRING`.
        - `new_value` (Required): The new value to replace existing values associated with the specified key within the JSON structure. This allows for dynamic updates to the JSON's content. Type should be `STRING`.
    - Outputs:
        - `json_output`: The updated JSON string, reflecting the changes made to values associated with the specified key. It represents the final state of the JSON after applying the updates. Type should be `STRING`.