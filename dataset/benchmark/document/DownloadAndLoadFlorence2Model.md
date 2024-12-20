- `DownloadAndLoadFlorence2Model`: This node is designed to download and load a specified Florence2 model, applying the chosen precision and attention mechanism settings. It ensures the model is ready for use by initializing it with the appropriate device, data type, and attention implementation.
    - Inputs:
        - `model` (Required): Specifies the repository ID of the Florence2 model to be downloaded and loaded. It influences the model's capabilities and features. Type should be `COMBO[STRING]`.
        - `precision` (Required): Determines the numerical precision (e.g., bf16, fp16, fp32) of the model's computations, affecting performance and memory usage. Type should be `COMBO[STRING]`.
        - `attention` (Required): Selects the attention mechanism implementation to be used by the model, impacting its performance and accuracy. Type should be `COMBO[STRING]`.
    - Outputs:
        - `florence2_model`: A dictionary containing the loaded model, its processor, and the data type used for computations. Type should be `FL2MODEL`.
