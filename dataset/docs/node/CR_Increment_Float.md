- `CR Increment Float`: The CR_IncrementFloat node is designed to incrementally adjust floating-point values, facilitating the creation of sequences or gradients of numbers. This node is particularly useful in scenarios where gradual changes or interpolations are required.
    - Parameters:
        - `start_value`: Specifies the initial value from which the incrementation starts, setting the baseline for the sequence generation. Type should be `FLOAT`.
        - `step`: Determines the increment size for each step, directly influencing the pace and scale of the sequence progression. Type should be `FLOAT`.
        - `start_frame`: Defines the starting frame for the incrementation process, marking the point at which the sequence begins. Type should be `INT`.
        - `frame_duration`: Specifies the duration in frames for each increment step, affecting the timing and pacing of the sequence. Type should be `INT`.
        - `current_frame`: Indicates the current frame in the sequence, used to calculate the current value based on the starting point and step size. Type should be `INT`.
    - Inputs:
    - Outputs:
        - `FLOAT`: Outputs the current incremented value, reflecting the progression of the sequence. Type should be `FLOAT`.
        - `show_help`: Provides additional information or guidance related to the node's operation. Type should be `STRING`.