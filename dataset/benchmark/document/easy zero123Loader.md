- `easy zero123Loader`: The easy zero123Loader node is designed to simplify the process of loading and configuring 3D models for use within the ComfyUI framework. It abstracts away the complexities involved in setting up 3D model parameters, making it easier for users to integrate 3D content into their applications.
    - Inputs:
        - `ckpt_name` (Required): Identifies the checkpoint name for the model to be loaded, serving as a key identifier for selecting the specific 3D model configuration. Type should be `COMBO[STRING]`.
        - `vae_name` (Required): Specifies the name of the VAE model to be used in conjunction with the 3D model, facilitating the generation or manipulation of 3D content. Type should be `COMBO[STRING]`.
        - `init_image` (Required): Provides an initial image to guide the generation or manipulation process, acting as a starting point for the 3D model's output. Type should be `IMAGE`.
        - `empty_latent_width` (Required): Defines the width of the latent space to be used for generating or manipulating 3D content, impacting the resolution and detail of the output. Type should be `INT`.
        - `empty_latent_height` (Required): Specifies the height of the latent space, influencing the vertical resolution and detail of the 3D model's output. Type should be `INT`.
        - `batch_size` (Required): Determines the number of instances to be processed in a single batch, affecting the efficiency and speed of the loading operation. Type should be `INT`.
        - `elevation` (Required): Sets the elevation angle for the 3D model's viewpoint, altering the vertical perspective of the rendered content. Type should be `FLOAT`.
        - `azimuth` (Required): Defines the azimuth angle, adjusting the horizontal orientation and perspective of the 3D model's output. Type should be `FLOAT`.
    - Outputs:
        - `pipe`: The pipeline object configured with the specified 3D model and settings, ready for use in generating or manipulating 3D content. Type should be `PIPE_LINE`.
        - `model`: The loaded 3D model object, prepared for integration and use within the ComfyUI framework. Type should be `MODEL`.
        - `vae`: The VAE model associated with the 3D model, enabling advanced content generation and manipulation capabilities. Type should be `VAE`.