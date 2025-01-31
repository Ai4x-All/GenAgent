- `FL_ImageDimensionDisplay`: This node is designed to calculate and display the dimensions of an image, supporting both individual images and batches of images in various formats. It abstracts the complexity of handling different image representations, providing a straightforward way to obtain image dimensions.
    - Inputs:
        - `image` (Required): The image input is crucial for determining the dimensions of the provided image. It supports both tensor and PIL image formats, adapting its processing based on the input type to accurately return the image dimensions. Type should be `IMAGE`.
    - Outputs:
        - `string`: Outputs the dimensions of the provided image as a string, formatted to include both width and height. Type should be `STRING`.
