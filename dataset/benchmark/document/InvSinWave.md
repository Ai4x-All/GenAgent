- `InvSinWave`: The InvSinWave node generates an inverse sine wave pattern, modifying the wave's amplitude based on the absolute value of the cosine function. It's designed for creating dynamic, wave-like animations or effects by adjusting parameters such as phase, amplitude, x translation, and y translation over a series of frames.
    - Inputs:
        - `phase` (Required): Defines the period of the wave, affecting how many units it takes for the wave to complete one full cycle. A crucial parameter for controlling the wave's speed and spacing. Type should be `FLOAT`.
        - `amplitude` (Required): Determines the height of the wave's peaks. This parameter influences the wave's intensity and the range of its vertical movement. Type should be `FLOAT`.
        - `x_translation` (Required): Shifts the wave along the x-axis, allowing for horizontal positioning adjustments. Type should be `FLOAT`.
        - `y_translation` (Required): Adjusts the wave's vertical positioning, allowing for vertical positioning adjustments. Type should be `FLOAT`.
        - `current_frame` (Required): Specifies the current frame in the animation sequence, enabling the wave pattern to evolve over time. Type should be `INT`.
    - Outputs:
        - `float`: Outputs the calculated wave value, useful for precise wave calculations. Type should be `FLOAT`.
        - `int`: Outputs the integer representation of the wave value, useful for scenarios requiring discrete values. Type should be `INT`.
