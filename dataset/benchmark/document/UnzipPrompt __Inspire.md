- `UnzipPrompt __Inspire`: The UnzipPrompt node is designed to decompress and separate a zipped prompt into its constituent parts, typically including positive, negative, and optional name components. This functionality is essential for processing and utilizing complex prompt structures within the InspirePack framework.
    - Inputs:
        - `zipped_prompt` (Required): The zipped_prompt parameter is the compressed form of the prompt that needs to be decompressed. It plays a crucial role in the node's operation by being the source data that is unpacked into its individual components. Type should be `ZIPPED_PROMPT`.
    - Outputs:
        - `positive`: The positive output represents the positive aspect of the decompressed prompt. Type should be `STRING`.
        - `negative`: The negative output represents the negative aspect of the decompressed prompt. Type should be `STRING`.
        - `name`: The name output represents the optional name component of the decompressed prompt, providing additional context or identification. Type should be `STRING`.
