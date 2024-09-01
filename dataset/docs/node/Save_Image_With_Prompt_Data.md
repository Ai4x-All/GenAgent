- `Save Image With Prompt Data`: This node is designed to save images along with associated prompt data and additional PNG metadata. It encapsulates the functionality to embed prompt information and other relevant metadata directly into the PNG files, facilitating a seamless integration of image content with descriptive data. The node aims to enhance the utility and interpretability of saved images by embedding contextual information, making it easier for users to understand and manage their image collections.
    - Parameters:
        - `positive_prompt`: The 'positive_prompt' parameter enables the inclusion of positive prompt information as part of the image's metadata, offering insights into the desired attributes or themes of the images. Type should be `STRING`.
        - `negative_prompt`: The 'negative_prompt' parameter allows for the inclusion of negative prompt information, specifying undesired attributes or themes to avoid in the images, enriching the contextual data. Type should be `STRING`.
        - `filename_prefix`: The 'filename_prefix' parameter allows users to specify a prefix for the filenames of the saved images. This aids in organizing and identifying images within a collection, providing a customizable naming convention that reflects the content or context of the images. Type should be `STRING`.
        - `parameters`: The 'parameters' parameter permits the inclusion of additional parameters as part of the image's metadata, further customizing the metadata content and enhancing the descriptive data of the images. Type should be `STRING`.
    - Inputs:
        - `images`: The 'images' parameter represents the collection of images to be saved. It is crucial for specifying the visual content that will be embedded with prompt data and additional metadata, serving as the primary input for the node's operation. Type should be `IMAGE`.
    - Outputs: