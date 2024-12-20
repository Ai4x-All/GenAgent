- `Multiply Float Float (JPS)`: Performs multiplication of two floating-point numbers, returning both integer and floating-point representations of the result. This node is designed to facilitate mathematical operations within a broader computational workflow, emphasizing flexibility in handling numerical data.
    - Inputs:
        - `float_a` (Required): Represents the first floating-point number to be multiplied. Its value influences the multiplication operation and the resulting output. Type should be `FLOAT`.
        - `float_b` (Required): Represents the second floating-point number to be multiplied. Together with float_a, it determines the outcome of the multiplication process. Type should be `FLOAT`.
    - Outputs:
        - `int_multiply`: The result of the multiplication operation cast to an integer, providing a whole number representation of the product. Type should be `INT`.
        - `float_multiply`: The result of the multiplication operation as a floating-point number, offering a precise representation of the product. Type should be `FLOAT`.
