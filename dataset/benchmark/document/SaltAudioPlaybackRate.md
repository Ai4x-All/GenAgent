- `SaltAudioPlaybackRate`: This node is designed to adjust the playback speed of an audio file. It allows users to increase or decrease the speed of audio playback without altering the pitch, providing a versatile tool for audio editing and manipulation.
    - Inputs:
        - `audio` (Required): The audio input is the raw audio data that the node will process to adjust its playback speed. It serves as the primary content for speed adjustment. Type should be `AUDIO`.
        - `speed_factor` (Required): The speed factor determines the rate at which the audio playback speed is adjusted. A value greater than 1 speeds up the playback, while a value less than 1 slows it down, offering precise control over the audio's tempo. Type should be `FLOAT`.
    - Outputs:
        - `audio`: The output is the modified audio data with the adjusted playback speed. It retains the original audio's pitch while altering its tempo. Type should be `AUDIO`.
