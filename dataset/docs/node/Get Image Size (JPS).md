- `Get Image Size (JPS)`: This node is designed to determine the dimensions of an image, specifically its width and height. It abstracts the process of analyzing an image's size, providing a straightforward way to obtain these fundamental attributes.
    - Parameters:
    - Inputs:
        - `image`: The image for which the size needs to be determined. This input is crucial as it directly influences the output by providing the necessary data to calculate the image's dimensions. Type should be `IMAGE`.
    - Outputs:
        - `width`: The width of the input image, measured in pixels. Type should be `INT`.
        - `height`: The height of the input image, measured in pixels. Type should be `INT`.