- `CR Math Operation`: The CR_MathOperation node performs a variety of mathematical operations on a given input value, such as trigonometric functions, square root, exponentiation, logarithm, negation, and absolute value. It allows for the specification of the operation to be performed and the number of decimal places for the result, making it a versatile tool for mathematical manipulations within the node network.
    - Parameters:
        - `a`: The input value on which the mathematical operation will be performed. The choice of operation affects the node's execution and the nature of the result. Type should be `FLOAT`.
        - `operation`: Specifies the mathematical operation to be applied to the input value. This determines the mathematical transformation that the input will undergo. Type should be `COMBO[STRING]`.
        - `decimal_places`: Determines the number of decimal places to which the result will be rounded. This allows for control over the precision of the output. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `a`: The result of the specified mathematical operation performed on the input value, rounded to the specified number of decimal places. Type should be `FLOAT`.
        - `show_help`: A URL to a help page providing detailed information about the mathematical operations supported by this node. Type should be `STRING`.