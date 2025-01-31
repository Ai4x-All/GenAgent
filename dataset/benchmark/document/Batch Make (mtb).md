- `Batch Make (mtb)`: The MTB_BatchMake node is designed to create batches from individual data points or smaller batches, facilitating the processing of data in bulk. This node is essential for optimizing data handling and processing efficiency in machine learning workflows, especially when dealing with large datasets or when performing operations that benefit from batch processing.
    - Inputs:
        - `image` (Required): This input type is used for specifying images that are to be batched together, playing a crucial role in the batch creation process for visual data. Type should be `IMAGE`.
        - `count` (Required): The 'count' input type specifies the number of images or data points to include in each batch, directly affecting the size and composition of the created batches. Type should be `INT`.
    - Outputs:
        - `image`: This output type represents batches of images, ready for further processing or analysis in downstream tasks. Type should be `IMAGE`.
