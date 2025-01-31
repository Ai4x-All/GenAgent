- `Conditioning Input Switch`: The Conditioning Input Switch node is designed to selectively switch between two conditioning inputs based on a boolean value, facilitating dynamic control over which conditioning data is passed forward in a processing pipeline.
    - Inputs:
        - `conditioning_a` (Required): The first conditioning input option. It serves as one of the two possible conditioning data inputs to be selected based on the boolean value. Type should be `CONDITIONING`.
        - `conditioning_b` (Required): The second conditioning input option. It acts as an alternative to the first conditioning input, offering a choice that can be selected based on the boolean value. Type should be `CONDITIONING`.
        - `boolean` (Required): A boolean value that determines which conditioning input (either conditioning_a or conditioning_b) is passed forward. When true, conditioning_a is selected; otherwise, conditioning_b is chosen. Type should be `BOOLEAN`.
    - Outputs:
        - `conditioning`: The selected conditioning input, determined by the boolean value. It outputs the chosen conditioning data for further processing. Type should be `CONDITIONING`.
