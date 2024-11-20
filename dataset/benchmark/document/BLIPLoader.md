- `BLIPLoader`: The BLIPLoader node is designed to load and initialize the BLIP model for image processing tasks. It encapsulates the complexities of setting up the BLIP model, including loading the pre-trained weights, configuring the model for inference, and ensuring it is ready to process images.
    - Inputs:
        - `model_name` (Required): Specifies the name of the BLIP model to load. This parameter determines which pre-trained model weights are loaded, affecting the node's performance and the quality of image processing. Type should be `COMBO[STRING]`.
    - Outputs:
        - `blip_model`: Returns an instance of the BLIP model, fully configured and ready for image processing tasks. This model can then be used to perform various image understanding and manipulation tasks. Type should be `BLIP_MODEL`.