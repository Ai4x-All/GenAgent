- `SeargeIntegerMath`: The SeargeIntegerMath node provides mathematical operations on integer values, supporting basic arithmetic functions such as addition, subtraction, multiplication, and division. It allows for the dynamic execution of predefined operations based on input parameters, facilitating various integer math computations.
    - Parameters:
        - `op`: Specifies the mathematical operation to be performed, chosen from a predefined set of operations. This determines how the input integers are processed and affects the outcome of the computation. Type should be `COMBO[STRING]`.
        - `a`: The first integer operand in the mathematical operation, serving as a primary input for the computation. Type should be `INT`.
        - `b`: The second integer operand, used in operations involving two inputs, such as multiplication or division. Type should be `INT`.
        - `c`: An optional third integer operand, used in operations that require an additional input, such as adding a constant after multiplication. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `result`: The integer result of the specified mathematical operation. Type should be `INT`.