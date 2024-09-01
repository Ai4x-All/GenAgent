- `ttN pipeKSampler`: The ttN_pipeKSampler node is designed to facilitate advanced sampling techniques for image generation, leveraging a combination of model inputs, sampling configurations, and image manipulation parameters. It abstracts the complexity of configuring and executing sampling processes, offering a streamlined interface for generating images with specific attributes or modifications.
    - Parameters:
        - `lora_name`: Specifies the LoRA model to be used, influencing the adaptation and fine-tuning of the generative model. Type should be `COMBO[STRING]`.
        - `lora_model_strength`: Determines the strength of the LoRA model's influence on the generative model, adjusting the degree of adaptation. Type should be `FLOAT`.
        - `lora_clip_strength`: Controls the strength of the LoRA model's influence on the CLIP model, adjusting semantic understanding. Type should be `FLOAT`.
        - `upscale_method`: Defines the method used for upscaling the generated images, affecting image resolution and quality. Type should be `COMBO[STRING]`.
        - `factor`: The factor by which the image is upscaled, directly impacting the final image size. Type should be `FLOAT`.
        - `crop`: Specifies the cropping parameters for the generated images, affecting the final image composition. Type should be `COMBO[STRING]`.
        - `sampler_state`: The state of the sampler used during the image generation process, influencing sampling behavior. Type should be `COMBO[STRING]`.
        - `steps`: The number of steps to run the sampling process, affecting the detail and quality of the generated images. Type should be `INT`.
        - `cfg`: The configuration guidance factor, influencing the coherence and quality of the generated images. Type should be `FLOAT`.
        - `sampler_name`: The name of the sampler algorithm used, determining the sampling technique. Type should be `COMBO[STRING]`.
        - `scheduler`: Specifies the scheduler for controlling the sampling process, affecting the progression of image generation. Type should be `COMBO[STRING]`.
        - `denoise`: The denoising factor applied during image generation, affecting image clarity and noise levels. Type should be `FLOAT`.
        - `image_output`: The output path for the generated images, determining where the images are saved. Type should be `COMBO[STRING]`.
        - `save_prefix`: A prefix added to the names of saved images, aiding in their organization and identification. Type should be `STRING`.
        - `seed`: The random seed used for the sampling process, ensuring reproducibility of the generated images. Type should be `INT`.
    - Inputs:
        - `pipe`: A structured input containing various configuration settings and model parameters for the sampling process. Type should be `PIPE_LINE`.
        - `optional_model`: An optional model parameter that allows for the specification of an alternative generative model. Type should be `MODEL`.
        - `optional_positive`: Optional positive prompts to guide the image generation towards desired themes or elements. Type should be `CONDITIONING`.
        - `optional_negative`: Optional negative prompts intended to steer the image generation away from certain themes or elements. Type should be `CONDITIONING`.
        - `optional_latent`: Optional initial latent space inputs for the generative model, serving as a starting point for the image generation process. Type should be `LATENT`.
        - `optional_vae`: An optional variational autoencoder used to enhance the image generation process. Type should be `VAE`.
        - `optional_clip`: An optional model used for semantic understanding of images and texts, aiding in aligning the generated images with the provided prompts. Type should be `CLIP`.
        - `xyPlot`: Specifies the parameters for generating an XY plot, potentially used for visualizing aspects of the sampling process. Type should be `XYPLOT`.
    - Outputs:
        - `pipe`: The updated pipe structure containing the results of the sampling process, including configurations and generated images. Type should be `PIPE_LINE`.
        - `model`: The generative model used in the sampling process, potentially modified by LoRA or other parameters. Type should be `MODEL`.
        - `positive`: The list of positive prompts used to guide the image generation process. Type should be `CONDITIONING`.
        - `negative`: The list of negative prompts used to refine the image generation process. Type should be `CONDITIONING`.
        - `latent`: The latent space representation resulting from the sampling process. Type should be `LATENT`.
        - `vae`: The variational autoencoder involved in the image generation process. Type should be `VAE`.
        - `clip`: The CLIP model used for semantic understanding in the sampling process. Type should be `CLIP`.
        - `image`: The final generated image or images resulting from the sampling process. Type should be `IMAGE`.
        - `seed`: The seed value used during the sampling process, influencing the randomness and reproducibility of results. Type should be `INT`.