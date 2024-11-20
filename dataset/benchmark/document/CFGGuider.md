- `CFGGuider`: The CFGGuider node is designed to guide the sampling process in generative models by applying conditional fine-grained control. It leverages conditioning inputs and a configurable control factor to steer the generation towards desired attributes or away from undesired ones, enhancing the model's ability to produce targeted outputs.
    - Inputs:
        - `model` (Required): The generative model to which the guidance will be applied. It serves as the foundation for the guidance process, determining the base behavior and capabilities of the guided sampling. Type should be `MODEL`.
        - `positive` (Required): A conditioning input intended to steer the model towards generating content that aligns with the specified attributes or themes. Type should be `CONDITIONING`.
        - `negative` (Required): A conditioning input used to steer the model away from generating content that aligns with the specified attributes or themes, acting as a counterbalance to the positive conditioning. Type should be `CONDITIONING`.
        - `cfg` (Required): A floating-point value that represents the strength of the conditional fine-grained control applied during the sampling process. It modulates the influence of the conditioning inputs on the generated output. Type should be `FLOAT`.
    - Outputs:
        - `guider`: The output is a configured guider object that encapsulates the logic and parameters for guiding the generative model's sampling process according to the specified conditions and control factor. Type should be `GUIDER`.