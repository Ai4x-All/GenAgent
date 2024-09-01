- `DualCLIPLoader`: The DualCLIPLoader node is designed for loading two CLIP models simultaneously, facilitating operations that require the integration or comparison of features from both models.
    - Parameters:
        - `clip_name1`: Specifies the name of the first CLIP model to be loaded. This parameter is crucial for identifying and retrieving the correct model from a predefined list of available CLIP models. Type should be `COMBO[STRING]`.
        - `clip_name2`: Specifies the name of the second CLIP model to be loaded. This parameter enables the loading of a second distinct CLIP model for comparative or integrative analysis alongside the first model. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `clip`: The output is a combined CLIP model that integrates the features or functionalities of the two specified CLIP models. Type should be `CLIP`.