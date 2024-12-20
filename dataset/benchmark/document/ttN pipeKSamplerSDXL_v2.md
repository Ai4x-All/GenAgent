- `ttN pipeKSamplerSDXL_v2`: This node is designed to facilitate the sampling process within a specific pipeline, focusing on handling and transforming data through various stages of sampling, including initialization, processing, and output generation. It abstracts the complexities involved in managing state, handling image outputs, and integrating with other components like models and samplers, aiming to streamline the workflow for generating and refining samples based on given inputs.
    - Inputs:
        - `sdxl_pipe` (Required): Represents the pipeline state or configuration that is being passed through the sampling process. It is crucial for maintaining continuity and consistency across different stages of sampling. Type should be `PIPE_LINE_SDXL`.
        - `lora_name` (Required): unknown Type should be `COMBO[STRING]`.
        - `lora_strength` (Required): unknown Type should be `FLOAT`.
        - `upscale_method` (Required): unknown Type should be `COMBO[STRING]`.
        - `upscale_model_name` (Required): unknown Type should be `COMBO[STRING]`.
        - `factor` (Required): unknown Type should be `FLOAT`.
        - `rescale` (Required): unknown Type should be `COMBO[STRING]`.
        - `percent` (Required): unknown Type should be `INT`.
        - `width` (Required): unknown Type should be `INT`.
        - `height` (Required): unknown Type should be `INT`.
        - `longer_side` (Required): unknown Type should be `INT`.
        - `crop` (Required): unknown Type should be `COMBO[STRING]`.
        - `base_steps` (Required): unknown Type should be `INT`.
        - `cfg` (Required): unknown Type should be `FLOAT`.
        - `denoise` (Required): unknown Type should be `FLOAT`.
        - `refiner_steps` (Required): unknown Type should be `INT`.
        - `refiner_cfg` (Required): unknown Type should be `FLOAT`.
        - `refiner_denoise` (Required): unknown Type should be `FLOAT`.
        - `sampler_name` (Required): unknown Type should be `COMBO[STRING]`.
        - `scheduler` (Required): unknown Type should be `COMBO[STRING]`.
        - `image_output` (Required): Specifies the desired output handling for images, such as whether to hide or save them, affecting how the node processes and returns image data. Type should be `COMBO[STRING]`.
        - `save_prefix` (Required): unknown Type should be `STRING`.
        - `file_type` (Required): unknown Type should be `COMBO[STRING]`.
        - `embed_workflow` (Required): unknown Type should be `BOOLEAN`.
        - `seed` (Optional): unknown Type should be `INT`.
        - `optional_model` (Optional): unknown Type should be `MODEL`.
        - `optional_positive` (Optional): unknown Type should be `CONDITIONING`.
        - `optional_negative` (Optional): unknown Type should be `CONDITIONING`.
        - `optional_latent` (Optional): unknown Type should be `LATENT`.
        - `optional_vae` (Optional): unknown Type should be `VAE`.
        - `optional_refiner_model` (Optional): unknown Type should be `MODEL`.
        - `optional_refiner_positive` (Optional): unknown Type should be `CONDITIONING`.
        - `optional_refiner_negative` (Optional): unknown Type should be `CONDITIONING`.
        - `optional_clip` (Optional): unknown Type should be `CLIP`.
        - `input_image_override` (Optional): unknown Type should be `IMAGE`.
        - `adv_xyPlot` (Optional): unknown Type should be `ADV_XYPLOT`.
    - Outputs:
        - `sdxl_pipe`: unknown Type should be `PIPE_LINE_SDXL`.
        - `pipe`: unknown Type should be `PIPE_LINE`.
        - `model`: unknown Type should be `MODEL`.
        - `positive`: unknown Type should be `CONDITIONING`.
        - `negative`: unknown Type should be `CONDITIONING`.
        - `refiner_model`: unknown Type should be `MODEL`.
        - `refiner_positive`: unknown Type should be `CONDITIONING`.
        - `refiner_negative`: unknown Type should be `CONDITIONING`.
        - `latent`: unknown Type should be `LATENT`.
        - `vae`: unknown Type should be `VAE`.
        - `clip`: unknown Type should be `CLIP`.
        - `images`: unknown Type should be `IMAGE`.
        - `seed`: unknown Type should be `INT`.
        - `plot_image`: unknown Type should be `IMAGE`.
