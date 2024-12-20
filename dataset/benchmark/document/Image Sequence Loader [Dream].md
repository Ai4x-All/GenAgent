- `Image Sequence Loader [Dream]`: The Image Sequence Loader node is designed to load a sequence of images from a specified directory, applying a pattern and indexing method to select the images. It can also provide a default image as a fallback option if no images are found matching the criteria.
    - Inputs:
        - `frame_counter` (Required): Represents the current frame counter, used to determine which image in the sequence to load based on its order. Type should be `FRAME_COUNTER`.
        - `directory_path` (Required): The path to the directory where the image sequence is stored. This allows the node to locate and load the images. Type should be `STRING`.
        - `pattern` (Required): A pattern to match filenames within the directory, enabling selective loading of images based on their names. Type should be `STRING`.
        - `indexing` (Required): Determines the method of indexing the images, either numerically or in alphabetical order, to establish the sequence order. Type should be `COMBO[STRING]`.
        - `default_image` (Optional): An optional default image to return if no images match the specified pattern and indexing in the directory. Type should be `IMAGE`.
    - Outputs:
        - `image`: The loaded image from the sequence based on the current frame counter, or the default image if no matching image is found. Type should be `IMAGE`.
        - `frame_name`: The name of the frame loaded from the sequence, providing context or identification for the image. Type should be `STRING`.
