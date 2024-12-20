- `SeargeFloatMath`: SeargeFloatMath provides mathematical operations on floating-point numbers, allowing for the execution of basic arithmetic operations with customizable operands and operation types.
    - Inputs:
        - `op` (Required): Specifies the arithmetic operation to be performed, chosen from a predefined list of operations. This affects the calculation result by determining which mathematical operation is applied. Type should be `COMBO[STRING]`.
        - `a` (Required): The first operand in the arithmetic operation, serving as a base value for calculations. Type should be `FLOAT`.
        - `b` (Required): The second operand, used in multiplication and division operations with the first operand. Type should be `FLOAT`.
        - `c` (Required): An additional operand used in operations involving addition or subtraction, enhancing the flexibility of calculations. Type should be `FLOAT`.
    - Outputs:
        - `result`: The result of the specified arithmetic operation performed on the input operands. Type should be `FLOAT`.
