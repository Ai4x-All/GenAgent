- `ImageDirIterator`: The ImageDirIterator node is designed to iterate through images in a specified directory, providing functionality to access and manipulate image files based on directory structure and file properties. This node is likely to facilitate operations such as image retrieval, sorting, and processing, aiming to streamline workflows that involve handling multiple images stored in a directory.
    - Inputs:
        - `directory_path` (Required): Specifies the path to the directory containing images. This path is used to locate and iterate through the image files for processing. Type should be `STRING`.
        - `image_index` (Required): An index to specify which image to retrieve from the sorted list of images in the directory. This allows for sequential or specific access to images. Type should be `INT`.
    - Outputs:
        - `image`: The image retrieved from the directory at the specified index, processed and returned as a tensor. Type should be `IMAGE`.
        - `string`: The filename of the retrieved image, without its extension, providing a means to identify or reference the image. Type should be `STRING`.