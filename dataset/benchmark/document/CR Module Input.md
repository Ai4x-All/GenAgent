- `CR Module Input`: The CR_ModuleInput node is designed to facilitate the flow of data through a pipeline by accepting a variety of inputs and flushing them through the system. It serves as a critical junction point in the pipeline, ensuring that data is correctly routed and transformed for subsequent processing stages.
    - Inputs:
        - `pipe` (Required): The 'pipe' parameter is the primary conduit for data flowing through the node. It encapsulates a variety of data types and structures, acting as a central hub for the input data that will be processed and routed within the pipeline. Type should be `PIPE_LINE`.
    - Outputs:
        - `pipe`: Represents the aggregated and processed data, ready to be forwarded to the next stage in the pipeline. Type should be `PIPE_LINE`.
        - `model`: The model data extracted from the input pipe. Type should be `MODEL`.
        - `pos`: Positive conditioning data extracted from the input pipe. Type should be `CONDITIONING`.
        - `neg`: Negative conditioning data extracted from the input pipe. Type should be `CONDITIONING`.
        - `latent`: Latent representation data extracted from the input pipe. Type should be `LATENT`.
        - `vae`: VAE model data extracted from the input pipe. Type should be `VAE`.
        - `clip`: CLIP model data extracted from the input pipe. Type should be `CLIP`.
        - `controlnet`: ControlNet data extracted from the input pipe. Type should be `CONTROL_NET`.
        - `image`: Image data extracted from the input pipe. Type should be `IMAGE`.
        - `seed`: Seed value extracted from the input pipe. Type should be `INT`.
        - `show_help`: A URL providing additional help and documentation for the node. Type should be `STRING`.
