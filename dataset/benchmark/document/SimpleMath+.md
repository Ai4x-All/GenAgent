- `SimpleMath+`: SimpleMath is a node designed to evaluate mathematical expressions dynamically. It interprets and computes expressions from abstract syntax trees (AST), supporting basic arithmetic operations, variable resolution, custom function calls, and array indexing.
    - Inputs:
        - `value` (Required): The mathematical expression to be evaluated, represented as a string. It is parsed into an abstract syntax tree (AST) for evaluation, supporting operations like addition, subtraction, multiplication, division, and more complex expressions involving variables and functions. Type should be `STRING`.
        - `a` (Optional): An optional variable 'a' that can be used within the mathematical expression. Its value affects the computation if 'a' is referenced in the expression. Type should be `INT,FLOAT`.
        - `b` (Optional): An optional variable 'b' that can be used within the mathematical expression. Its value affects the computation if 'b' is referenced in the expression. Type should be `INT,FLOAT`.
    - Outputs:
        - `int`: The rounded integer result of the evaluated mathematical expression. Type should be `INT`.
        - `float`: The exact floating-point result of the evaluated mathematical expression. Type should be `FLOAT`.
