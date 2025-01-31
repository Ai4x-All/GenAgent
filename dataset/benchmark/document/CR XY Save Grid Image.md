- `CR XY Save Grid Image`: This node is designed to save a grid of images to a specified output path, optionally adding annotations to the images. It supports various file formats and allows for customization of image saving parameters such as compression level and quality. The node can operate in different modes, such as saving for output or generating a temporary preview, and provides a UI component for previewing the saved images.
    - Inputs:
        - `mode` (Required): Specifies the operation mode of the node, which can be either 'Save' for saving images to a permanent location or 'Preview' for generating temporary images for preview purposes. This affects the type of path used for saving and the metadata associated with the saved images. Type should be `COMBO[STRING]`.
        - `output_folder` (Required): The name of the folder where the images will be saved. This folder is created inside a predefined output directory. Type should be `COMBO[STRING]`.
        - `image` (Required): The image or images to be saved. This can be a single image or a list of images to be arranged in a grid. Type should be `IMAGE`.
        - `filename_prefix` (Required): A prefix added to the filename of the saved images, useful for organizing and identifying images. Type should be `STRING`.
        - `file_format` (Required): The file format in which the images will be saved. Supports common formats like PNG, JPG, WEBP, and TIFF. Type should be `COMBO[STRING]`.
        - `output_path` (Optional): An optional custom path where the images will be saved. If provided, it overrides the default output folder path. Type should be `STRING`.
        - `trigger` (Optional): A boolean flag that must be set to True to activate the image saving process. If False, the node does not perform any action. Type should be `BOOLEAN`.
    - Outputs:
