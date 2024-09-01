- `Prompt With SDXL`: The Prompt With SDXL node is designed to process and encode textual prompts with specific styles for image generation, utilizing both positive and negative prompts. It integrates with the CLIPTextEncodeSDXL and CLIPTextEncodeSDXLRefiner for encoding, and applies various transformations including syntax stripping, metadata addition, and condition encoding to prepare the prompts for the image generation process.
    - Parameters:
        - `positive_prompt`: The positive prompt is a textual input that describes desired attributes or elements to be included in the generated image. It plays a crucial role in guiding the image generation process towards the intended outcome. Type should be `STRING`.
        - `negative_prompt`: The negative prompt specifies undesired attributes or elements to be excluded from the generated image. It helps in refining the output by preventing the inclusion of specified elements, thus enhancing the relevance of the generated image. Type should be `STRING`.
        - `positive_style`: Specifies the style to be applied to the positive prompt, influencing the aesthetic and thematic direction of the generated image. Type should be `STRING`.
        - `negative_style`: Specifies the style to be applied to the negative prompt, influencing the aesthetic and thematic direction of the generated image by excluding certain styles. Type should be `STRING`.
        - `ratio_selected`: Determines the aspect ratio for the generated image, influencing its dimensions. Type should be `COMBO[STRING]`.
        - `batch_size`: Specifies the number of images to be generated in a single batch, allowing for bulk processing. Type should be `INT`.
        - `seed`: The seed parameter is used to ensure reproducibility in the image generation process. It initializes the random number generator, allowing for consistent results across multiple runs with the same inputs. Type should be `INT`.
        - `output_option`: Defines how the prompts and styles are combined and encoded for the image generation process. Type should be `COMBO[STRING]`.
    - Inputs:
    - Outputs:
        - `samples`: The generated image samples based on the processed and encoded prompts. Type should be `LATENT`.
        - `positive_prompt_text_g`: The processed positive prompt text for the 'g' channel encoding. Type should be `STRING`.
        - `negative_prompt_text_g`: The processed negative prompt text for the 'g' channel encoding. Type should be `STRING`.
        - `positive_style_text_l`: The processed positive style text for the 'l' channel encoding. Type should be `STRING`.
        - `negative_style_text_l`: The processed negative style text for the 'l' channel encoding. Type should be `STRING`.
        - `width`: The width of the generated image. Type should be `INT`.
        - `height`: The height of the generated image. Type should be `INT`.
        - `refiner_width`: The width of the image after refinement. Type should be `INT`.
        - `refiner_height`: The height of the image after refinement. Type should be `INT`.