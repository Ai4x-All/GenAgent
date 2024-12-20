- `LLMImageVisionLLMReader`: The LLMImageVisionLLMReader node is designed to read and process image files, leveraging large language models (LLMs) to interpret and extract information from visual content. It aims to bridge the gap between visual data and textual analysis, enabling a deeper understanding of images through the lens of LLMs.
    - Inputs:
        - `path` (Required): Specifies the file path to the image to be processed. It is a crucial parameter as it determines the source of the visual data the node will analyze. Type should be `STRING`.
        - `extra_info` (Optional): Provides additional, optional information in a string format that can be used to influence the processing of the image. This could include settings or parameters specific to the task at hand. Type should be `STRING`.
    - Outputs:
        - `documents`: Returns the processed data as documents, encapsulating the insights extracted from the image by the LLM. Type should be `DOCUMENT`.
