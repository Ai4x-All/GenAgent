- `AbsCosWave`: The AbsCosWave node generates a wave pattern based on the absolute value of a cosine function, modulated by parameters such as phase, amplitude, x_translation, and max_value. It's designed to create dynamic, visually interesting waveforms for various applications.
    - Inputs:
        - `phase` (Required): The phase parameter controls the periodicity of the wave, affecting how frequently the wave pattern repeats over a given interval. Type should be `FLOAT`.
        - `amplitude` (Required): Amplitude determines the height of the wave peaks, influencing the overall intensity of the wave pattern. Type should be `FLOAT`.
        - `x_translation` (Required): X_translation shifts the wave pattern along the horizontal axis, allowing for adjustments in the wave's starting position. Type should be `FLOAT`.
        - `max_value` (Required): Max_value sets the upper limit for the wave's value, capping the peak height and affecting the wave's amplitude. Type should be `FLOAT`.
        - `current_frame` (Required): Current_frame represents a specific point in time or sequence, used to calculate the wave's position and shape at that moment. Type should be `INT`.
    - Outputs:
        - `float`: The first element of the output tuple, representing the calculated wave value in its precise form. Type should be `FLOAT`.
        - `int`: The second element of the output tuple, providing an integer approximation of the wave's current state. Type should be `INT`.
