- `easy cascadeLoader`: The `easy cascadeLoader` node is designed to facilitate the loading and management of cascading models, specifically focusing on integrating multiple model stages for enhanced processing capabilities. It abstracts the complexity of handling various model stages, making it easier to implement sophisticated model cascading strategies within the ComfyUI framework.
    - Inputs:
        - `stage_c` (Required): Specifies the combined list of filenames from the 'unet' and 'cascade' model directories. This input is crucial for determining the sequence and composition of models to be loaded for cascading operations, directly influencing the loader's behavior and the resulting model integration. Type should be `COMBO[STRING]`.
        - `stage_b` (Required): Represents the filenames for the second stage of the cascading models, playing a critical role in the sequential processing and integration of model stages. Type should be `COMBO[STRING]`.
        - `stage_a` (Required): Denotes the filenames for the initial stage of the cascading models, essential for setting up the foundational processing layer in the cascading strategy. Type should be `COMBO[STRING]`.
        - `clip_name` (Required): Specifies the filenames for the CLIP models to be used in conjunction with the cascading models, enhancing the model's understanding and processing capabilities. Type should be `COMBO[STRING]`.
        - `lora_name` (Required): Specifies the LoRA model names available for enhancing the model's capabilities, particularly in terms of adaptability and fine-tuning. Type should be `COMBO[STRING]`.
        - `lora_model_strength` (Required): Determines the strength of the LoRA model adjustments, influencing the model's performance and adaptability. Type should be `FLOAT`.
        - `lora_clip_strength` (Required): Sets the strength of the CLIP adjustments when LoRA models are used, affecting the overall model performance. Type should be `FLOAT`.
        - `resolution` (Required): Defines the resolution for the model's output, impacting the quality and detail of the generated images. Type should be `COMBO[STRING]`.
        - `empty_latent_width` (Required): Specifies the width of the empty latent space, crucial for initializing the model's processing capabilities. Type should be `INT`.
        - `empty_latent_height` (Required): Determines the height of the empty latent space, essential for the model's initial setup and processing. Type should be `INT`.
        - `compression` (Required): Sets the level of compression for the model's output, balancing between quality and efficiency. Type should be `INT`.
        - `positive` (Required): Captures positive prompts or keywords to guide the model's generation process towards desired outcomes. Type should be `STRING`.
        - `negative` (Required): Includes negative prompts or keywords to steer the model away from undesired elements in the generation process. Type should be `STRING`.
        - `batch_size` (Required): Specifies the number of instances to be processed in a single batch, affecting the model's efficiency and throughput. Type should be `INT`.
        - `optional_lora_stack` (Optional): Allows for the optional inclusion of a stack of LoRA models, offering enhanced customization and fine-tuning capabilities. Type should be `LORA_STACK`.
    - Outputs:
        - `pipe`: The pipeline object that orchestrates the flow and integration of various model stages. Type should be `PIPE_LINE`.
        - `model_c`: The model object for the final stage in the cascading process, ready for further operations or analysis. Type should be `MODEL`.
        - `latent_c`: The latent representation generated by the final stage model, capturing the processed information. Type should be `LATENT`.
        - `vae`: The VAE model used in the cascading process, contributing to the generation or processing of data. Type should be `VAE`.