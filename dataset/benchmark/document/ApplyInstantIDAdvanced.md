- `ApplyInstantIDAdvanced`: The ApplyInstantIDAdvanced node is designed to enhance image generation with specific identity features by applying advanced conditioning techniques. It utilizes a combination of InstantID, insight face analysis, control net adjustments, and additional parameters to fine-tune the identity preservation and control in the generated images.
    - Inputs:
        - `instantid` (Required): The InstantID parameter is crucial for providing the identity-specific features to be preserved or emphasized in the generated image. Type should be `INSTANTID`.
        - `insightface` (Required): Insightface parameter is used for face analysis, providing critical facial feature information that aids in the identity preservation process. Type should be `FACEANALYSIS`.
        - `control_net` (Required): Control net parameter allows for fine-tuning and control over the generation process, ensuring the identity features are accurately applied. Type should be `CONTROL_NET`.
        - `image` (Required): The image parameter serves as the base for identity application, where the identity features are to be preserved or emphasized. Type should be `IMAGE`.
        - `model` (Required): Model parameter specifies the generative model to be used in conjunction with identity features for image generation. Type should be `MODEL`.
        - `positive` (Required): Positive conditioning to emphasize certain identity features in the generated image. Type should be `CONDITIONING`.
        - `negative` (Required): Negative conditioning to de-emphasize certain identity features in the generated image. Type should be `CONDITIONING`.
        - `ip_weight` (Required): IP weight parameter adjusts the influence of identity preservation in the generation process. Type should be `FLOAT`.
        - `cn_strength` (Required): CN strength parameter controls the strength of the control net adjustments in the identity application process. Type should be `FLOAT`.
        - `start_at` (Required): Start at parameter defines the beginning point of identity feature application in the generation process. Type should be `FLOAT`.
        - `end_at` (Required): End at parameter defines the end point of identity feature application in the generation process. Type should be `FLOAT`.
        - `noise` (Required): Noise parameter introduces variability in the identity features application, enhancing the naturalness of the generated image. Type should be `FLOAT`.
        - `combine_embeds` (Required): Combine embeds parameter determines the method of combining multiple identity embeddings for application in the image generation. Type should be `COMBO[STRING]`.
        - `image_kps` (Optional): Image keypoints parameter provides additional facial feature information for enhanced identity preservation. Type should be `IMAGE`.
        - `mask` (Optional): Mask parameter allows for selective application of identity features in the generated image, enhancing control over the preservation process. Type should be `MASK`.
    - Outputs:
        - `MODEL`: The output model after applying InstantIDAdvanced, incorporating the identity features and adjustments made through the input parameters. Type should be `MODEL`.
        - `positive`: The enhanced positive conditioning output, reflecting the emphasized identity features in the generated image. Type should be `CONDITIONING`.
        - `negative`: The enhanced negative conditioning output, reflecting the de-emphasized identity features in the generated image. Type should be `CONDITIONING`.