- `easy LLLiteLoader`: The `easy LLLiteLoader` node is designed to simplify the process of loading and integrating LLLite models into a user's workflow. It abstracts the complexities involved in handling model files, setting up the necessary configurations, and ensuring compatibility with the broader system, thereby making it easier for users to leverage LLLite models for their specific tasks.
    - Inputs:
        - `model` (Required): Specifies the model to be loaded, focusing on the selection from a predefined list of available models, which is essential for the loading process. Type should be `MODEL`.
        - `model_name` (Required): Determines the specific name of the model to be loaded, allowing for precise identification and retrieval of the model file. Type should be `COMBO[STRING]`.
        - `cond_image` (Required): Indicates the conditional image to be used in conjunction with the model, affecting the model's output based on the provided image. Type should be `IMAGE`.
        - `strength` (Required): Defines the strength of the effect to be applied by the model, allowing users to control the intensity of the model's output. Type should be `FLOAT`.
        - `steps` (Required): Specifies the number of steps to be used in the model's processing, affecting the detail and quality of the output. Type should be `INT`.
        - `start_percent` (Required): Sets the starting percentage for the model's processing, allowing for partial application of the model's effects. Type should be `FLOAT`.
        - `end_percent` (Required): Determines the ending percentage for the model's processing, enabling fine-tuning of the model's application range. Type should be `FLOAT`.
    - Outputs:
        - `model`: Outputs the loaded model, ready for use in the user's workflow, encapsulating the model's functionalities and configurations. Type should be `MODEL`.
