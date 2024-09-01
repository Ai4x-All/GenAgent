- `CR Image List`: The CR Image List node is designed to load and process a list of images from a specified directory, converting them into a format suitable for further manipulation or analysis. It focuses on organizing and preparing image data by ensuring the images are in a consistent format and facilitating their use in subsequent operations.
    - Parameters:
        - `alias1`: An alias for the first image, providing a means to reference it more conveniently in subsequent operations. Type should be `STRING`.
        - `alias2`: An alias for the second image, aiding in its identification and use in later stages. Type should be `STRING`.
        - `alias3`: An alias for the third image, facilitating easier reference and manipulation. Type should be `STRING`.
        - `alias4`: An alias for the fourth image, simplifying its identification and subsequent processing. Type should be `STRING`.
        - `alias5`: An alias for the fifth image, making it easier to refer to and work with in further operations. Type should be `STRING`.
    - Inputs:
        - `image_1`: Specifies the first image to be processed. This parameter is part of a series that allows for the loading and processing of multiple images. Type should be `IMAGE`.
        - `image_2`: Specifies the second image to be processed, following the same pattern as the first. Type should be `IMAGE`.
        - `image_3`: Specifies the third image to be processed, continuing the sequence of image inputs. Type should be `IMAGE`.
        - `image_4`: Specifies the fourth image to be processed, extending the list of images to be handled. Type should be `IMAGE`.
        - `image_5`: Specifies the fifth image to be processed, completing the series of image inputs. Type should be `IMAGE`.
        - `image_list`: A list parameter that allows for the bulk loading and processing of images, accommodating larger sets of image data. Type should be `image_LIST`.
    - Outputs:
        - `IMAGE_LIST`: A list of images that have been loaded and converted to a consistent format, ready for further processing or analysis. Type should be `IMAGE_LIST`.
        - `show_help`: Provides a link to helpful documentation or resources related to the node's functionality. Type should be `STRING`.