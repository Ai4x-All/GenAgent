- `LoadAndApplyICLightUnet`: This node is designed to load and apply IC-Light Unet weights to a model, ensuring compatibility with specific model architectures by patching and converting state dictionaries as necessary. It focuses on enhancing models with IC-Light Unet's capabilities, facilitating the integration of advanced lighting effects into generated images.
    - Inputs:
        - `model` (Required): The model to which IC-Light Unet weights will be applied. It plays a crucial role in the node's operation by being the recipient of the enhanced lighting capabilities provided by IC-Light Unet. Type should be `MODEL`.
        - `model_path` (Required): The path to the IC-Light Unet weights file. This parameter is essential for locating and loading the specific weights to be applied to the model. Type should be `COMBO[STRING]`.
    - Outputs:
        - `model`: The model enhanced with IC-Light Unet weights. This output is crucial for utilizing the model with advanced lighting effects in generated images. Type should be `MODEL`.