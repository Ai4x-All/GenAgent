- `easy ipadapterApplyFromParams`: This node facilitates the application of IPAdapter parameters to a model, streamlining the process of integrating and customizing image processing adaptations. It abstracts the complexity of applying various IPAdapter configurations, making it easier for users to enhance their models with advanced image manipulation capabilities.
    - Inputs:
        - `model` (Required): The model to which the IPAdapter parameters will be applied. It serves as the base for further image processing enhancements. Type should be `MODEL`.
        - `preset` (Required): Specifies the preset configuration for the IPAdapter application, influencing the adaptation process. Type should be `COMBO[STRING]`.
        - `ipadapter_params` (Required): A collection of parameters and configurations for the IPAdapter, detailing how image processing should be adapted. Type should be `IPADAPTER_PARAMS`.
        - `combine_embeds` (Required): Determines how embeddings are combined during the adaptation process, affecting the final image output. Type should be `COMBO[STRING]`.
        - `embeds_scaling` (Required): Defines how embeddings are scaled, impacting the adaptation's influence on the image processing. Type should be `COMBO[STRING]`.
        - `cache_mode` (Required): Controls the caching behavior during the adaptation process, optimizing performance and resource usage. Type should be `COMBO[STRING]`.
        - `optional_ipadapter` (Optional): An optional IPAdapter instance that can be applied in addition to the primary adapter, for layered adaptations. Type should be `IPADAPTER`.
        - `image_negative` (Optional): Optional negative image embeddings to be applied, offering a way to negate certain attributes in the model's output. Type should be `IMAGE`.
    - Outputs:
        - `model`: The enhanced model with applied IPAdapter parameters, ready for further processing or utilization. Type should be `MODEL`.
        - `ipadapter`: The IPAdapter instance after application to the model, reflecting the updated configurations and parameters. Type should be `IPADAPTER`.
