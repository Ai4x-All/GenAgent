- `JWImageLoadRGB`: This node is designed to load an image from a specified path and convert it into an RGB format. It abstracts the complexities of image file handling and conversion, providing a straightforward way to work with image data in RGB format.
    - Inputs:
        - `path` (Required): Specifies the file path of the image to be loaded. This parameter is crucial as it determines which image file the node will process and convert to RGB format. Type should be `STRING`.
    - Outputs:
        - `image`: The output is the image data converted into RGB format, ready for further processing or visualization. Type should be `IMAGE`.
