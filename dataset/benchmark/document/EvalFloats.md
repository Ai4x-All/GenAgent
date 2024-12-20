- `EvalFloats`: EvalFloats is designed to dynamically evaluate mathematical expressions provided by the user. It takes two float inputs and a formula as a string, processes the formula by substituting the inputs, and returns the result in multiple formats.
    - Inputs:
        - `a` (Required): Represents the first float input for the mathematical formula. Its value is crucial as it directly influences the outcome of the evaluated expression. Type should be `FLOAT`.
        - `b` (Required): Serves as the second float input for the mathematical formula. Similar to 'a', its value significantly affects the result of the expression. Type should be `FLOAT`.
        - `formula` (Required): A string input representing the mathematical formula to be evaluated. This formula should include placeholders for 'a' and 'b' which are replaced by their respective input values during processing. Type should be `STRING`.
    - Outputs:
        - `result_float`: The floating-point result of the evaluated mathematical formula. Type should be `FLOAT`.
