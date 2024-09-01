- `JWImageSaveToPath`: This node is designed to save a single image to a specified path, optionally embedding additional metadata such as a prompt or other PNG-specific information within the image file.
    - Parameters:
        - `path`: Specifies the file system path where the image will be saved. This path determines the location and filename of the output image. Type should be `STRING`.
    - Inputs:
        - `image`: The image data to be saved. This tensor represents the image in a format that can be processed and saved to the specified path. Type should be `IMAGE`.
        - `overwrite`: A flag indicating whether an existing file at the specified path should be overwritten. If set to 'true', the existing file will be replaced with the new image. Type should be `['false', 'true']`.
    - Outputs: