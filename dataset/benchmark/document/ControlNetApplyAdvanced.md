- `ControlNetApplyAdvanced`: This node is designed for advanced application of a control network to modify the conditioning of an image generation process. It leverages a control network to adjust the conditioning based on the provided image, strength, and additional parameters, enhancing the control over the generation outcome.
    - Inputs:
        - `positive` (Required): The positive conditioning data that the control network will modify, representing the desired attributes or features to emphasize in the generated image. Type should be `CONDITIONING`.
        - `negative` (Required): The negative conditioning data that the control network will modify, representing the attributes or features to de-emphasize or avoid in the generated image. Type should be `CONDITIONING`.
        - `control_net` (Required): The control network model used to apply modifications to the conditioning. It is central to the node's functionality, enabling the dynamic adjustment of the generation process. Type should be `CONTROL_NET`.
        - `image` (Required): The image data that influences the control network's modifications to the conditioning. It serves as a contextual basis for the adjustments. Type should be `IMAGE`.
        - `strength` (Required): A scalar value that determines the intensity of the control network's modifications. It allows for fine-tuning the impact of the control network on the conditioning. Type should be `FLOAT`.
        - `start_percent` (Required): The starting percentage of the control effect, allowing for gradual application of the control network's influence over the image generation process. Type should be `FLOAT`.
        - `end_percent` (Required): The ending percentage of the control effect, defining the point at which the control network's influence ceases, enabling precise control over the conditioning modification. Type should be `FLOAT`.
    - Outputs:
        - `positive`: The modified positive conditioning data after the control network's application, reflecting the desired adjustments. Type should be `CONDITIONING`.
        - `negative`: The modified negative conditioning data after the control network's application, reflecting the de-emphasized or avoided attributes. Type should be `CONDITIONING`.