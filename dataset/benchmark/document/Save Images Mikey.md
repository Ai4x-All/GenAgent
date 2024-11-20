- `Save Images Mikey`: This node is designed to facilitate the saving of images to disk, incorporating additional functionalities such as prefixing filenames and appending extra information to PNG files. It abstracts the complexities involved in file handling and metadata management, aiming to streamline the process of persisting images with contextual data.
    - Inputs:
        - `images` (Required): The collection of images to be saved. This parameter is central to the node's operation, determining the primary content that will be persisted to disk. Type should be `IMAGE`.
        - `sub_directory` (Required): Specifies the sub-directory within the output folder where the images will be saved, aiding in the organization of saved files. Type should be `STRING`.
        - `filename_text_i` (Required): The part of the dynamic filename construction, contributing to a customizable naming scheme. This parameter allows for multiple filename texts to be specified, enhancing the flexibility in naming saved images. Type should be `STRING`.
        - `filename_separator` (Required): A separator character or string used between different parts of the filename to ensure readability and structure. Type should be `STRING`.
        - `timestamp` (Required): Indicates whether a timestamp should be included in the filename, providing a time-based identifier for the saved image. Type should be `COMBO[STRING]`.
        - `counter_type` (Required): Defines the type of counter to be used in the filename, aiding in the creation of unique filenames for each saved image. Type should be `COMBO[STRING]`.
        - `filename_text_i_pos` (Required): unknown Type should be `INT`.
        - `timestamp_pos` (Required): The position in the filename where the timestamp should be inserted, if applicable, to incorporate time-based identifiers. Type should be `INT`.
        - `timestamp_type` (Required): Specifies the format of the timestamp to be included in the filename, ensuring consistency in time-based identifiers. Type should be `COMBO[STRING]`.
        - `counter_pos` (Required): The position in the filename where the counter should be inserted, facilitating the generation of unique filenames. Type should be `INT`.
        - `extra_metadata` (Required): Additional metadata that can be included with the image, enhancing the documentation and traceability of the saved file. Type should be `STRING`.
    - Outputs: