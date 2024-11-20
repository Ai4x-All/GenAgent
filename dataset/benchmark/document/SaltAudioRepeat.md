- `SaltAudioRepeat`: The SaltAudioRepeat node is designed for repeating an audio segment a specified number of times. It enables the creation of looped audio effects by duplicating the input audio according to the user-defined repetition count.
    - Inputs:
        - `audio` (Required): The 'audio' parameter is the raw audio data to be looped. It is essential for determining the base audio content that will be repeated. Type should be `AUDIO`.
        - `repeat_times` (Required): The 'repeat_times' parameter specifies how many times the audio should be looped. It directly influences the length and content of the output audio. Type should be `INT`.
    - Outputs:
        - `audio`: The output is the looped audio, which is the result of repeating the input audio segment for the specified number of times. Type should be `AUDIO`.