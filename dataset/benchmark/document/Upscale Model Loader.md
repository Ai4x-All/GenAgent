- `Upscale Model Loader`: This node is designed to load and prepare upscale models for use, ensuring they are in the correct state for upscaling tasks. It handles the intricacies of loading model state dictionaries and adjusting them if necessary, streamlining the process of getting models ready for image enhancement operations.
    - Inputs:
        - `model_name` (Required): Specifies the name of the upscale model to be loaded. This name is used to locate the model file within a predefined directory structure, facilitating the retrieval and loading of the model for upscaling purposes. Type should be `COMBO[STRING]`.
    - Outputs:
        - `UPSCALE_MODEL`: The loaded and prepared upscale model, ready for use in upscaling tasks. This output facilitates the enhancement of images by providing a model that has been properly configured and evaluated. Type should be `UPSCALE_MODEL`.
        - `MODEL_NAME_TEXT`: The name of the loaded upscale model, provided as text. This output is useful for identifying or referencing the model that has been loaded and prepared for use. Type should be `STRING`.
