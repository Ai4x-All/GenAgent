- `ImageCrop+`: The ImageCrop+ node is designed for cropping images to a specified width and height starting from a given x and y coordinate. It allows for precise control over the portion of the image to be extracted, making it a fundamental tool for image manipulation and preprocessing tasks.
    - Inputs:
        - `image` (Required): The input image to be cropped. This parameter is crucial as it defines the source image from which a specific region will be extracted. Type should be `IMAGE`.
        - `width` (Required): Specifies the width of the cropped image. It determines how wide the resulting image will be after cropping. Type should be `INT`.
        - `height` (Required): Specifies the height of the cropped image. It determines the vertical size of the resulting image after cropping. Type should be `INT`.
        - `position` (Required): Defines the starting position for the crop operation, offering predefined options for alignment. Type should be `COMBO[STRING]`.
        - `x_offset` (Required): The horizontal offset from the specified position for additional control over the cropping area. Type should be `INT`.
        - `y_offset` (Required): The vertical offset from the specified position for additional control over the cropping area. Type should be `INT`.
    - Outputs:
        - `IMAGE`: The cropped portion of the input image. This output is the direct result of the cropping operation, representing the specified region of the original image. Type should be `IMAGE`.
        - `x`: The x-coordinate of the top-left corner of the cropped image. Type should be `INT`.
        - `y`: The y-coordinate of the top-left corner of the cropped image. Type should be `INT`.
