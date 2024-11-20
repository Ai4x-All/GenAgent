- `SaltLayerExtractor`: The SaltLayerExtractor node is designed for extracting specific layer data from a sequence of animation layers based on a given index. It focuses on isolating zoom, x, and y values for a particular layer, facilitating the creation of detailed animation schedules for parallax motion effects.
    - Inputs:
        - `float_layers` (Required): A list of animation layers, where each layer is represented as a sequence of frames with float values for zoom, x, and y positions. This input is crucial for determining the specific layer data to extract. Type should be `LIST`.
        - `layer_index` (Required): An integer specifying the index of the layer to extract from the list of animation layers. This determines which layer's data is processed and extracted. Type should be `INT`.
    - Outputs:
        - `zoom_schedule_lsit`: unknown Type should be `LIST`.
        - `x_schedule_list`: A list of x position values extracted from the specified layer, representing the horizontal movement schedule for animation. Type should be `LIST`.
        - `y_schedule_list`: A list of y position values extracted from the specified layer, representing the vertical movement schedule for animation. Type should be `LIST`.