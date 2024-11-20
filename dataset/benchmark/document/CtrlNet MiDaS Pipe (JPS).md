- `CtrlNet MiDaS Pipe (JPS)`: The CtrlNet MiDaS Pipe node is designed to process settings for depth estimation using the MiDaS model, encapsulating the configuration into a format suitable for further processing or application within a pipeline. It primarily serves to adjust depth-related parameters based on input settings.
    - Inputs:
        - `midas_settings` (Required): Specifies the configuration for depth estimation, including source, strength, start, end, and additional parameters, which collectively determine how depth estimation is performed. Type should be `BASIC_PIPE`.
    - Outputs:
        - `midas_source`: Identifies the source image for depth estimation. Type should be `INT`.
        - `midas_strength`: Specifies the strength of the depth effect. Type should be `FLOAT`.
        - `midas_start`: Defines the starting point of depth effect application. Type should be `FLOAT`.
        - `midas_end`: Marks the end point of depth effect application. Type should be `FLOAT`.
        - `midas_a`: Adjusts a specific depth parameter, influencing the overall depth effect. Type should be `FLOAT`.
        - `midas_bg`: Controls the background depth parameter, affecting how background depth is rendered. Type should be `FLOAT`.