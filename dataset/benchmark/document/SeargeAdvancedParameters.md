- `SeargeAdvancedParameters`: The SeargeAdvancedParameters node is designed to handle and process advanced configuration parameters for the generation process. It allows for the customization and fine-tuning of generation settings, enabling users to adjust parameters that influence the output's quality, style, and other advanced aspects.
    - Inputs:
        - `dynamic_cfg_method` (Required): unknown Type should be `COMBO[STRING]`.
        - `dynamic_cfg_factor` (Required): unknown Type should be `FLOAT`.
        - `refiner_detail_boost` (Required): unknown Type should be `FLOAT`.
        - `contrast_factor` (Required): unknown Type should be `FLOAT`.
        - `saturation_factor` (Required): unknown Type should be `FLOAT`.
        - `latent_detailer` (Required): unknown Type should be `COMBO[STRING]`.
        - `data` (Optional): unknown Type should be `SRG_DATA_STREAM`.
    - Outputs:
        - `data`: This output represents the processed data stream, encapsulating all the adjusted and fine-tuned parameters for the generation process. Type should be `SRG_DATA_STREAM`.
