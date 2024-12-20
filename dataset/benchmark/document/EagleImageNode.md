- `EagleImageNode`: The EagleImageNode is designed for processing and handling image sequences, particularly focusing on adjusting images to a uniform size, converting them to a consistent format, and preparing them for further processing or analysis. It emphasizes the manipulation of image data, including resizing, format conversion, and mask generation, to facilitate downstream tasks such as image composition or analysis.
    - Inputs:
        - `image` (Required): Specifies the image to be processed, essential for performing operations such as resizing, format conversion, and mask generation. Type should be `IMAGE`.
        - `int_field` (Required): An integer parameter that influences the node's processing logic, such as defining the dimensions for resizing or the number of iterations for certain operations, directly impacting the output's characteristics. Type should be `INT`.
        - `float_field` (Required): A floating-point parameter that may adjust the intensity or threshold levels of certain image processing functions, affecting the visual outcome of the processed image. Type should be `FLOAT`.
        - `print_to_screen` (Required): A boolean parameter that controls the verbosity of the node's operation, determining whether intermediate or final processing results are displayed to the user. Type should be `COMBO[STRING]`.
        - `string_field` (Required): A string parameter that could specify file paths, format types, or other textual configurations relevant to the node's processing tasks. Type should be `STRING`.
    - Outputs:
