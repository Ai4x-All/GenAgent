- `CM_Vec2ToScalarUnaryOperation`: This node performs a unary operation that transforms a 2-dimensional vector into a scalar value, based on a specified operation. It abstracts complex mathematical operations into a simple interface, allowing for the transformation of vector data into a single numerical outcome.
    - Inputs:
        - `op` (Required): Specifies the unary operation to be performed on the vector, determining the nature of the transformation from a 2D vector to a scalar value. Type should be `COMBO[STRING]`.
        - `a` (Required): The 2-dimensional vector to be transformed into a scalar value through the specified operation. Type should be `VEC2`.
    - Outputs:
        - `float`: The scalar result of the unary operation performed on the input 2-dimensional vector. Type should be `FLOAT`.
