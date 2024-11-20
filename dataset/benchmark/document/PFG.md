- `PFG`: The PFG node is designed to enhance the conditioning process in generative models by applying a learned transformation to the input conditioning vectors. It leverages a pre-trained model to compute features from an input image, which are then scaled and combined with the original conditioning vectors to produce modified conditioning vectors that better guide the generation process.
    - Inputs:
        - `positive` (Required): A conditioning vector representing the desired attributes or content in the generated output. It plays a crucial role in guiding the generative model towards producing outputs that align with the specified positive conditions. Type should be `CONDITIONING`.
        - `negative` (Required): A conditioning vector representing undesired attributes or content. It is used to steer the generative model away from generating outputs with these negative conditions. Type should be `CONDITIONING`.
        - `pfg_scale` (Required): A scaling factor for the PFG feature vector, allowing for adjustment of its influence on the conditioning process. This parameter fine-tunes how strongly the PFG-modified features affect the final generated output. Type should be `FLOAT`.
        - `image` (Required): The input image from which features are extracted using the PFG model. These features are then used to modify the conditioning vectors, enhancing the model's ability to generate desired outputs. Type should be `IMAGE`.
        - `model_name` (Required): The name of the pre-trained PFG model to use for feature extraction. This allows for flexibility in choosing different models based on the specific requirements or characteristics of the input image. Type should be `COMBO[STRING]`.
    - Outputs:
        - `conditioning`: The modified conditioning vectors, both positive and negative, enhanced with features extracted from the input image to better guide the generative process. Type should be `CONDITIONING`.