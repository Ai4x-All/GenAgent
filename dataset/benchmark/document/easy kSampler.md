- `easy kSampler`: The `easy kSampler` node simplifies the sampling process in generative models by providing a streamlined interface for generating images. It abstracts complex sampling configurations and parameters, offering users an easier way to produce high-quality image outputs.
    - Inputs:
        - `pipe` (Required): Specifies the pipeline configuration for the sampling process, determining how input data is processed and how outputs are generated. Type should be `PIPE_LINE`.
        - `image_output` (Required): Controls the output behavior of the sampling process, including whether to preview, save, or send the generated images. Type should be `COMBO[STRING]`.
        - `link_id` (Required): A unique identifier for the link in the pipeline, used to manage and track the flow of data. Type should be `INT`.
        - `save_prefix` (Required): Defines a prefix for saved image files, allowing for organized storage and easy retrieval. Type should be `STRING`.
        - `model` (Optional): Specifies the generative model used for sampling. This parameter is optional, allowing for flexibility in model selection. Type should be `MODEL`.
    - Outputs:
        - `pipe`: Represents the updated pipeline configuration after the sampling process, reflecting any changes or adjustments made. Type should be `PIPE_LINE`.
        - `image`: The generated image as a result of the sampling process, which can be previewed, saved, or sent based on the specified output behavior. Type should be `IMAGE`.
