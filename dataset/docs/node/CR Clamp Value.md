- `CR Clamp Value`: The CR Clamp Value node is designed to restrict a given value within a specified range, ensuring that the output value does not exceed the defined minimum and maximum limits. This functionality is crucial for maintaining data integrity and preventing errors in downstream processes that rely on bounded inputs.
    - Parameters:
        - `a`: The value to be clamped. It is the primary input whose final output is constrained within the specified range. Type should be `FLOAT`.
        - `range_min`: The minimum allowable value for the input. If 'a' is less than this value, 'a' is set to this minimum value. Type should be `FLOAT`.
        - `range_max`: The maximum allowable value for the input. If 'a' is greater than this value, 'a' is set to this maximum value. Type should be `FLOAT`.
    - Inputs:
    - Outputs:
        - `a`: The clamped value, adjusted to fall within the specified range. Type should be `FLOAT`.
        - `show_help`: A URL to the node's documentation, providing additional help and examples. Type should be `STRING`.