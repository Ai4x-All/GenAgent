- `CR Random RGB`: This node generates a set of four random RGB color values and provides a link to further help or documentation. It's designed to introduce variability and customization in visual elements by leveraging randomness.
    - Inputs:
        - `seed` (Required): The seed parameter initializes the random number generator, ensuring reproducibility of the random RGB colors generated. It plays a crucial role in enabling consistent results across different executions. Type should be `INT`.
    - Outputs:
        - `rgb_1`: A randomly generated RGB color value. Type should be `STRING`.
        - `rgb_2`: A randomly generated RGB color value. Type should be `STRING`.
        - `rgb_3`: A randomly generated RGB color value. Type should be `STRING`.
        - `rgb_4`: A randomly generated RGB color value. Type should be `STRING`.
        - `show_help`: A URL link to the node's documentation or help page. Type should be `STRING`.