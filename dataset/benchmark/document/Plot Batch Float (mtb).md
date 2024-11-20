- `Plot Batch Float (mtb)`: The MTB_PlotBatchFloat node is designed for visualizing batches of floating-point numbers as images. It generates plots based on the provided float values, allowing for a graphical representation of data distributions or patterns.
    - Inputs:
        - `width` (Required): Specifies the width of the generated plot image. Affects the resolution and size of the output image. Type should be `INT`.
        - `height` (Required): Specifies the height of the generated plot image. Influences the resolution and size of the output visualization. Type should be `INT`.
        - `point_size` (Required): Determines the size of each point in the plot. Larger values produce bigger points, enhancing visibility but potentially reducing clarity in dense areas. Type should be `INT`.
        - `seed` (Required): A seed value for random number generation, ensuring reproducibility of the plot's layout when using random elements. Type should be `INT`.
        - `start_at_zero` (Required): A boolean flag that, when true, forces the plot's axis to start at zero, potentially altering the plot's scale and appearance. Type should be `BOOLEAN`.
    - Outputs:
        - `plot`: The generated plot image, visualizing the input float values as a graphical representation. Type should be `IMAGE`.