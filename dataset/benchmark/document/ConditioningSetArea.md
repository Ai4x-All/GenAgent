- `ConditioningSetArea`: This node specializes in adjusting the conditioning of an image generation process by setting specific areas with defined dimensions and strength. It allows for precise control over the conditioning's spatial attributes, enabling targeted modifications to the generated image's characteristics within specified regions.
    - Inputs:
        - `conditioning` (Required): The conditioning input represents the current state of the image generation process, which this node modifies by setting specific areas. Type should be `CONDITIONING`.
        - `width` (Required): Specifies the width of the area to be set, allowing for precise spatial control within the conditioning. Type should be `INT`.
        - `height` (Required): Defines the height of the area to be set, contributing to the spatial specificity of the conditioning modification. Type should be `INT`.
        - `x` (Required): The x-coordinate of the top-left corner of the area to be set, positioning the modification within the conditioning. Type should be `INT`.
        - `y` (Required): The y-coordinate of the top-left corner of the area to be set, positioning the modification within the conditioning. Type should be `INT`.
        - `strength` (Required): Determines the intensity of the conditioning modification within the specified area, affecting the generated image's characteristics. Type should be `FLOAT`.
    - Outputs:
        - `conditioning`: The modified conditioning, with specific areas set according to the provided dimensions and strength, ready for further processing in the image generation pipeline. Type should be `CONDITIONING`.
