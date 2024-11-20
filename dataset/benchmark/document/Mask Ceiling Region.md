- `Mask Ceiling Region`: This node specializes in identifying and isolating the ceiling regions within given mask images. It leverages specific image processing techniques to discern and extract the ceiling areas, making it a valuable tool for tasks requiring focused analysis or manipulation of ceiling elements in images.
    - Inputs:
        - `masks` (Required): The input masks represent the images from which the ceiling regions are to be extracted. These masks are crucial for the node's operation as they serve as the basis for identifying and isolating ceiling areas. Type should be `MASK`.
    - Outputs:
        - `MASKS`: The output is a tensor of masks specifically highlighting the ceiling regions within the original input images. This allows for targeted analysis or manipulation of these areas. Type should be `MASK`.