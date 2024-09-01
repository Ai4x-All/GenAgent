- `CM_Vec3UnaryOperation`: The CM_Vec3UnaryOperation node performs unary operations on 3-dimensional vectors, applying a specified operation to a single vector and producing a modified vector as a result. This node abstracts the complexity of vector manipulation, enabling efficient and straightforward vector transformations.
    - Parameters:
        - `op`: Specifies the unary operation to be performed on the vector. The choice of operation directly influences the outcome of the transformation. Type should be `COMBO[STRING]`.
    - Inputs:
        - `a`: The 3-dimensional vector to be transformed. It serves as the input for the unary operation, determining the base vector for the transformation. Type should be `VEC3`.
    - Outputs:
        - `vec3`: The result of applying the specified unary operation to the input vector, represented as a 3-dimensional vector. Type should be `VEC3`.