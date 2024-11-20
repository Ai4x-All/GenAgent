- `easy imageScaleDownToSize`: This node provides functionality for scaling down images to a specified size while maintaining the aspect ratio. It allows users to choose between scaling down to the maximum or minimum dimension of the image, ensuring the final image dimensions do not exceed the specified size.
    - Inputs:
        - `images` (Required): The input images to be scaled down. This parameter is crucial for defining the source images that the scaling operation will be applied to. Type should be `IMAGE`.
        - `size` (Required): The target size to scale down the images to. This parameter determines the maximum dimension (width or height) of the output images, depending on the mode selected. Type should be `INT`.
        - `mode` (Required): A boolean flag indicating the scaling mode: 'max' to scale down based on the larger dimension or 'min' to scale based on the smaller dimension. This affects how the aspect ratio is preserved during scaling. Type should be `BOOLEAN`.
    - Outputs:
        - `image`: The output images after scaling down to the specified size, with aspect ratio maintained. Type should be `IMAGE`.