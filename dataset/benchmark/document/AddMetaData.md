- `AddMetaData`: The AddMetaData node is designed to embed metadata into images by associating specific labels and text values with them. This process enriches the image data with additional, descriptive information that can be utilized for various purposes, such as categorization, identification, or further processing.
    - Inputs:
        - `image` (Required): The image to which metadata will be added. It serves as the primary input for the metadata embedding process. Type should be `IMAGE`.
        - `label` (Required): A label that categorizes or identifies the metadata being added. It acts as a key in the metadata dictionary. Type should be `STRING`.
        - `text_value` (Required): The actual text to be added as metadata under the specified label. This value enriches the image with descriptive or identifying information. Type should be `STRING`.
    - Outputs:
        - `image`: The image with the newly added metadata, allowing for enriched data representation and usage. Type should be `IMAGE`.
