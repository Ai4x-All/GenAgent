- `BboxToInt`: The BboxToInt node is designed to convert bounding box coordinates from a list format to individual integer values, including the calculation of the center points. This functionality is essential for applications requiring precise spatial locations and dimensions of objects within images.
    - Inputs:
        - `bboxes` (Required): The 'bboxes' parameter represents the list of bounding boxes to be processed. Each bounding box is expected to be a tuple or list containing the coordinates and dimensions of a rectangular area within an image. Type should be `BBOX`.
        - `index` (Required): The 'index' parameter specifies the position of the bounding box in the 'bboxes' list that should be converted to integer values. This allows for selective processing of bounding boxes. Type should be `INT`.
    - Outputs:
        - `x_min`: The minimum x-coordinate of the selected bounding box. Type should be `INT`.
        - `y_min`: The minimum y-coordinate of the selected bounding box. Type should be `INT`.
        - `width`: The width of the selected bounding box. Type should be `INT`.
        - `height`: The height of the selected bounding box. Type should be `INT`.
        - `center_x`: The x-coordinate of the center point of the selected bounding box. Type should be `INT`.
        - `center_y`: The y-coordinate of the center point of the selected bounding box. Type should be `INT`.