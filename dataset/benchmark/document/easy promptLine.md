- `easy promptLine`: The `easy promptLine` node is designed to facilitate the manipulation and conditioning of textual prompts for generative models. It enables the dynamic integration and adjustment of negative conditioning phrases, ensuring that the generated content aligns with specified constraints and preferences. This node plays a crucial role in refining the input prompts to achieve desired outcomes in generative tasks, such as text generation or image synthesis, by allowing for precise control over the conditioning process.
    - Inputs:
        - `prompt` (Required): Represents the primary textual content that the user inputs for processing. It serves as the base for any manipulations, additions, or exclusions applied by the node. Type should be `STRING`.
        - `start_index` (Required): Specifies the starting index from which the node begins to process the input prompt, allowing for segmented or partial processing of the text. Type should be `INT`.
        - `max_rows` (Required): Defines the maximum number of rows or lines to be processed or generated from the input prompt, setting a limit on the output's extent. Type should be `INT`.
    - Outputs:
        - `STRING`: The processed text output, which may include modifications, additions, or exclusions based on the node's functionality. Type should be `STRING`.
        - `COMBO`: A combination of processed text outputs, potentially including multiple variations or manipulations of the input prompt. Type should be `*`.
