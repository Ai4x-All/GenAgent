- `Color (RGB)`: This node is designed for creating a color representation from individual red, green, and blue components. It allows for the precise specification of colors in RGB format, facilitating their use in various image processing and visualization tasks.
    - Inputs:
        - `r` (Required): Specifies the red component of the color, contributing to the overall hue when combined with green and blue components. Type should be `INT`.
        - `g` (Required): Specifies the green component of the color, contributing to the overall hue when combined with red and blue components. Type should be `INT`.
        - `b` (Required): Specifies the blue component of the color, contributing to the overall hue when combined with red and green components. Type should be `INT`.
    - Outputs:
        - `color`: The RGB representation of the input components, allowing for its use in various image processing and visualization contexts. Type should be `COLOR`.