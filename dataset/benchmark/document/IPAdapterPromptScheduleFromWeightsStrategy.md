- `IPAdapterPromptScheduleFromWeightsStrategy`: This node generates a prompt schedule based on a given weights strategy, dynamically adjusting the prompt sequence to align with the specified frame count and incorporating optional starting and ending frames. It's designed to tailor the prompt delivery in image processing tasks, ensuring that prompts are optimally distributed across the desired number of frames.
    - Inputs:
        - `weights_strategy` (Required): A strategy dictating the distribution of weights across frames, including the total number of frames, and whether to add starting or ending frames. This strategy influences how the prompt schedule is generated, ensuring alignment with the frame-based processing requirements. Type should be `WEIGHTS_STRATEGY`.
        - `prompt` (Required): A multiline string input that represents the base prompt to be scheduled. This input is split and adjusted according to the weights strategy to fit the frame count, enhancing the relevance of the prompt at each frame. Type should be `STRING`.
    - Outputs:
        - `prompt_schedule`: A string representation of the scheduled prompts, formatted to align with the frame distribution specified by the weights strategy. This schedule is ready for use in frame-based image processing tasks. Type should be `STRING`.