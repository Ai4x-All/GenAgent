- `Range Integer`: The RangeInteger node is designed to generate a list of integers within a specified range, using a step value derived from a seed. It then selects an integer from this list based on an offset calculated from the seed, providing a way to deterministically select a number within a range.
    - Parameters:
        - `start`: Specifies the starting point of the range. It is crucial for defining the lower bound of the generated list of numbers. Type should be `INT`.
        - `end`: Defines the end point of the range, setting the upper limit for the list of integers to be generated. Type should be `INT`.
        - `step`: Determines the interval between each number in the range. It is derived from the seed value, adding a layer of determinism to the selection process. Type should be `INT`.
        - `seed`: Used as a basis for calculating the step value and the offset for selecting the final number. It introduces a deterministic element to the number selection. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `int`: The integer selected from the generated list based on the seed-derived offset. Type should be `INT`.
        - `string`: A string representation of the selected integer, providing a textual format of the output. Type should be `STRING`.