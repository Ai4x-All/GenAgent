- `CM_FloatBinaryCondition`: This node evaluates binary conditions between two floating-point numbers based on a specified operation. It abstracts the complexity of various floating-point comparisons into a simple interface, allowing users to perform mathematical comparisons like equality, inequality, greater than, and less than operations.
    - Inputs:
        - `op` (Required): Specifies the operation to perform on the two floating-point numbers. It determines the type of comparison (e.g., equal, not equal, greater than) to be executed. Type should be `COMBO[STRING]`.
        - `a` (Required): The first floating-point number to be compared. Type should be `FLOAT`.
        - `b` (Required): The second floating-point number to be compared. Type should be `FLOAT`.
    - Outputs:
        - `bool`: The result of the binary condition operation, indicating whether the specified condition between the two floating-point numbers is true or false. Type should be `BOOL`.
