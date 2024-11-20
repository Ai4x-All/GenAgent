- `Save Image Grid (mtb)`: The Save Image Grid node is designed to compile a collection of images into a single, cohesive grid layout. This functionality is particularly useful for visualizing multiple images in a structured format, allowing for easier comparison and analysis of visual data.
    - Inputs:
        - `images` (Required): A batch of images to be compiled into a grid. This collection is essential for determining the composition and overall appearance of the final image grid. Type should be `IMAGE`.
        - `filename_prefix` (Required): A prefix for the filename under which the grid image will be saved. This parameter allows for customizable naming of the output file, aiding in organization and retrieval. Type should be `STRING`.
        - `save_intermediate` (Required): A boolean flag indicating whether intermediate images should be saved during the grid compilation process. This option provides flexibility in saving individual images before they are combined into the final grid. Type should be `BOOLEAN`.
    - Outputs: