- `SaltScheduleConverter`: The SaltScheduleConverter node is designed to transform schedule lists into formats compatible with various modules by converting list elements into floats or integers. This ensures interoperability with modules that require specific numeric types, facilitating seamless integration and data manipulation within scheduling contexts.
    - Inputs:
        - `schedule_list` (Required): The 'schedule_list' parameter is a list of numeric values representing a schedule. It is essential for the conversion process, as it undergoes transformation into floats or integers, depending on the context, to ensure compatibility with other modules. Type should be `LIST`.
    - Outputs:
        - `floats`: A list of floats, representing the original schedule list without modification. Type should be `FLOATS`.
        - `float`: A duplicate of the 'floats' list, serving as a redundant output for compatibility purposes. Type should be `FLOAT`.
        - `int`: A list of integers, derived from rounding the values of the original schedule list, to accommodate modules requiring integer inputs. Type should be `INT`.