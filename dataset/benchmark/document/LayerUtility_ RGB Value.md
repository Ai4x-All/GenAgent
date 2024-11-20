- `LayerUtility_ RGB Value`: This node converts a given color value, either in hexadecimal string format or as an RGB tuple, into its constituent red, green, and blue (RGB) integer components. It's designed to facilitate color manipulation and analysis within image processing tasks by providing a direct way to extract and work with individual color channels.
    - Inputs:
        - `color_value` (Required): The color value input can be a hexadecimal string or an RGB tuple, representing the color to be converted into its RGB components. This input is crucial for determining the specific RGB values to be extracted, directly affecting the node's output. Type should be `*`.
    - Outputs:
        - `R`: The red component of the color, extracted as an integer value. Type should be `INT`.
        - `G`: The green component of the color, extracted as an integer value. Type should be `INT`.
        - `B`: The blue component of the color, extracted as an integer value. Type should be `INT`.