- `ModelSamplingContinuousV`: This node is designed to enhance a given model by applying a continuous variable (V) sampling technique, which involves cloning the original model and integrating a specialized sampling mechanism based on the 'v_prediction' method. It adjusts the model's behavior through dynamic sigma parameters, enabling refined control over the sampling process.
    - Inputs:
        - `model` (Required): The model to be enhanced with continuous variable sampling. It serves as the foundation for applying the sampling technique. Type should be `MODEL`.
        - `sampling` (Required): Specifies the sampling strategy to be used, which in this case is fixed to 'v_prediction', indicating the use of a prediction-based approach for continuous variable sampling. Type should be `COMBO[STRING]`.
        - `sigma_max` (Required): The maximum sigma value for the sampling process, allowing for the adjustment of the sampling's upper bound. Type should be `FLOAT`.
        - `sigma_min` (Required): The minimum sigma value for the sampling process, enabling the setting of the sampling's lower bound. Type should be `FLOAT`.
    - Outputs:
        - `model`: The enhanced model with the applied continuous variable (V) sampling technique, featuring the integrated specialized sampling mechanism. Type should be `MODEL`.
