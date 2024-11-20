- `ColorDictionary (custom)`: This node allows for the creation of a custom color dictionary by mapping user-defined color names to their corresponding color values. It ensures that the number of color names matches the number of color values, adjusting the lists to match in length if necessary, before returning a dictionary that associates each color name with its color value.
    - Inputs:
        - `color_names` (Required): A list of user-defined names for colors. These names are used as keys in the resulting color dictionary, allowing for easy identification and retrieval of color values. Type should be `STRING`.
        - `colors` (Required): A list of color values (typically RGB tuples) that correspond to the user-defined color names. These values are used as the dictionary values in the resulting color dictionary, mapping each name to its respective color. Type should be `COLOR`.
    - Outputs:
        - `color_dict`: The resulting custom color dictionary, mapping each user-defined color name to its corresponding color value. Type should be `COLOR_DICT`.