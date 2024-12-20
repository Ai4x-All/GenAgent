- `ModelPassThrough`: The ModelPassThrough node is designed to seamlessly forward a model input without any modifications. This functionality serves as a workaround for scenarios where bypassing inputs directly is not supported, ensuring that the model data can flow through the node unchanged.
    - Inputs:
        - `model` (Required): The model input represents the model data that will be passed through unchanged. It is crucial for maintaining the integrity of the model's structure and data throughout the node's operation. Type should be `MODEL`.
    - Outputs:
        - `model`: The output model is identical to the input model, having been passed through the node without any alterations. This ensures the model's structure and data remain intact for subsequent operations. Type should be `MODEL`.
