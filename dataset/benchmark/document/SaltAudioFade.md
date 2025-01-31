- `SaltAudioFade`: The SaltAudioFade node applies a fade-in or fade-out effect to an audio clip, based on specified parameters such as fade type, duration, and start time. This node is designed to manipulate the dynamics of an audio segment, enhancing its auditory transitions.
    - Inputs:
        - `audio` (Required): The raw audio data to which the fade effect will be applied. This is the primary input for the fade operation. Type should be `AUDIO`.
        - `fade_type` (Required): Specifies the type of fade effect to apply: 'in' for a fade-in effect, or 'out' for a fade-out effect. This determines the direction of the volume transition. Type should be `COMBO[STRING]`.
        - `fade_duration` (Required): The duration of the fade effect in seconds. This defines how long the fade transition will last. Type should be `FLOAT`.
        - `fade_start` (Optional): The start time in seconds for the fade effect. This optional parameter allows for specifying when the fade effect should begin within the audio clip. Type should be `FLOAT`.
    - Outputs:
        - `audio`: The modified audio data with the applied fade effect. This output is suitable for further processing or playback. Type should be `AUDIO`.
