- `SaltKeyframeVisualizer`: The SaltKeyframeVisualizer node is designed to visualize the keyframe scheduling process, providing a graphical representation of keyframe values across frames. It calculates various metrics for the keyframes within a specified frame range and generates a visualization image that highlights these metrics, aiding in the analysis and adjustment of keyframe-based animations.
    - Inputs:
        - `schedule_list` (Required): A list of keyframe values to be visualized. It is crucial for understanding the distribution and variation of keyframe values across the specified frame range, impacting the visualization's accuracy and detail. Type should be `LIST`.
        - `start_frame` (Optional): The starting frame number for the visualization. It defines the initial point of the frame range to be visualized, affecting the scope of the keyframe analysis. Type should be `INT`.
        - `end_frame` (Optional): The ending frame number for the visualization. It marks the boundary of the frame range to be analyzed and visualized, determining the extent of the keyframe metrics calculation. Type should be `INT`.
        - `simulate_stereo` (Optional): Indicates whether to simulate stereo visualization for the keyframes, adding a dimensional aspect to the analysis by mirroring keyframe values. Type should be `BOOLEAN`.
        - `frame_rate` (Optional): The frame rate used to calculate the duration of the keyframe sequence. It influences the time-based metrics and the overall temporal context of the visualization. Type should be `INT`.
        - `schedule_list_a` (Optional): An alternative list of keyframe values, providing additional context or variations for visualization. Type should be `LIST`.
        - `schedule_list_b` (Optional): Another variation of keyframe values list, offering further insights or comparative analysis in the visualization. Type should be `LIST`.
        - `schedule_list_c` (Optional): A third variation of keyframe values list, allowing for a broader range of comparative visualization and analysis. Type should be `LIST`.
    - Outputs: