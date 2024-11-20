- `Int to Log Entry [Dream]`: The 'Int to Log Entry' node is designed to convert an integer value along with an optional label into a log entry format. This functionality is essential for logging and tracking integer values within a system, providing a structured and readable log entry that can be easily interpreted and analyzed.
    - Inputs:
        - `value` (Required): The 'value' parameter represents the integer value to be logged. It is a crucial component of the log entry, serving as the primary data point around which the log entry is structured. Type should be `INT`.
        - `label` (Required): The 'label' parameter is an optional string that provides context or a descriptor for the integer value being logged. It enhances the readability and interpretability of the log entry by adding a textual description to the numerical value. Type should be `STRING`.
    - Outputs:
        - `log_entry`: The output 'log_entry' is a structured representation of the input integer value and optional label, formatted for logging purposes. It encapsulates the data in a log entry format, making it suitable for tracking and analysis within a logging system. Type should be `LOG_ENTRY`.