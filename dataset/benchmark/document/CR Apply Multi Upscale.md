- `CR Apply Multi Upscale`: This node is designed to apply multiple upscaling models sequentially to an image, enhancing its resolution. It allows for the customization of the upscaling process through a stack of models and rescaling factors, providing flexibility in achieving the desired image quality.
    - Inputs:
        - `image` (Required): The input image to be upscaled. It serves as the base for the sequential application of multiple upscaling models, each potentially enhancing the image's resolution further. Type should be `IMAGE`.
        - `resampling_method` (Required): Specifies the method used for resampling during the upscaling process, affecting the quality and characteristics of the upscaled image. Type should be `COMBO[STRING]`.
        - `supersample` (Required): Determines whether supersampling is applied, which can enhance the quality of the upscaled image by reducing aliasing effects. Type should be `COMBO[STRING]`.
        - `rounding_modulus` (Required): Used to round the dimensions of the upscaled image, ensuring they are multiples of a specified value, which can be important for compatibility with certain processing or display requirements. Type should be `INT`.
        - `upscale_stack` (Required): A list of tuples, each containing an upscaling model and a rescale factor. This stack defines the sequence and parameters of upscaling models applied to the image, allowing for complex and customized upscaling processes. Type should be `UPSCALE_STACK`.
    - Outputs:
        - `IMAGE`: The output of the node is the upscaled image, which has undergone sequential upscaling and potential resizing based on the provided stack of models and rescaling factors. Type should be `IMAGE`.
        - `show_help`: A URL providing additional information and guidance on the use of the node and its parameters. Type should be `STRING`.
