- `AdjustRect`: The AdjustRect node is designed to modify the dimensions of a rectangle based on specified parameters, ensuring the new rectangle adheres to certain constraints like center alignment and size adjustments. It abstracts the complexity of geometric transformations, offering a straightforward way to recalibrate rectangle dimensions for various applications.
    - Inputs:
        - `a` (Required): Represents one of the coordinates (x or y) of the rectangle, contributing to defining its initial position. Type should be `INT`.
        - `b` (Required): Represents another coordinate (x or y) of the rectangle, working alongside 'a' to specify the rectangle's starting dimensions. Type should be `INT`.
        - `c` (Required): Defines one of the dimensions (width or height) of the rectangle, influencing its size before adjustment. Type should be `INT`.
        - `d` (Required): Defines another dimension (width or height) of the rectangle, used in conjunction with 'c' to determine the initial size. Type should be `INT`.
        - `xm` (Required): Specifies the factor by which the rectangle's width is adjusted, ensuring the new width is a multiple of this value. Type should be `INT`.
        - `ym` (Required): Specifies the factor by which the rectangle's height is adjusted, ensuring the new height is a multiple of this value. Type should be `INT`.
        - `round_mode` (Required): Determines the rounding method used when adjusting the rectangle's dimensions, affecting the precision of the adjustment. Type should be `COMBO[STRING]`.
        - `input_format` (Required): Indicates the format of the input rectangle coordinates, dictating how they should be interpreted and transformed. Type should be `COMBO[STRING]`.
        - `output_format` (Required): Specifies the format for the output rectangle coordinates, determining how the adjusted dimensions are represented. Type should be `COMBO[STRING]`.
    - Outputs:
        - `int`: Each element of the output tuple represents a coordinate or dimension of the adjusted rectangle, reflecting the modifications applied to the original dimensions. The output is a tuple of integers, each specifying a part of the rectangle's adjusted geometry. Type should be `INT`.
