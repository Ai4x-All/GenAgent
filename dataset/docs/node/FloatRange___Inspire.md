- `FloatRange __Inspire`: The FloatRange node generates a sequence of floating-point numbers starting from a specified value, stopping at another, and incrementing by a defined step. It is designed to create custom ranges with precision control, including the option to ensure the final value is included in the sequence.
    - Parameters:
        - `start`: Defines the starting point of the range. It sets the initial value from which the sequence begins. Type should be `FLOAT`.
        - `stop`: Specifies the stopping point of the range. The sequence is generated up to this value, depending on the 'ensure_end' flag. Type should be `FLOAT`.
        - `step`: Determines the increment between each number in the sequence, allowing for fine-grained control over the range's progression. Type should be `FLOAT`.
        - `limit`: Limits the number of elements in the generated sequence to prevent excessive output. Type should be `INT`.
        - `ensure_end`: When enabled, ensures the stopping value is included in the sequence, adjusting the sequence if necessary. Type should be `BOOLEAN`.
    - Inputs:
    - Outputs:
        - `float`: A list of floating-point numbers constituting the generated range. This output is a list, which aligns with the expectation of a sequence of 'float' types. Type should be `FLOAT`.