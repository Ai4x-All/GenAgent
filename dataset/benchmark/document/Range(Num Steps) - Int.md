- `Range(Num Steps) - Int`: This node generates a range of integer values based on specified start and stop points, a number of steps, and an end mode. It allows for the creation of evenly or unevenly spaced sequences of integers, with options to include or exclude the stop point in the final range.
    - Inputs:
        - `start` (Required): Defines the starting point of the range. It sets the initial value from which the range begins. Type should be `INT`.
        - `stop` (Required): Sets the ending point of the range. This value can be included or excluded from the final range based on the end mode. Type should be `INT`.
        - `num_steps` (Required): Specifies the number of steps (or values) to generate within the range. It determines how many integers will be included in the sequence. Type should be `INT`.
        - `end_mode` (Required): Determines whether the stop point is included ('Inclusive') or excluded ('Exclusive') from the generated range. Type should be `COMBO[STRING]`.
        - `allow_uneven_steps` (Required): Indicates whether to allow steps that result in uneven spacing between the integers in the range. Type should be `COMBO[STRING]`.
    - Outputs:
        - `range`: The generated sequence of integers within the specified range. Type should be `INT`.
        - `range_sizes`: The size of each generated range, indicating how many integers are in each sequence. Type should be `INT`.