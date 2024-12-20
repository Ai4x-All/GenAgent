- `SaltMaskThresholdRegion`: This node applies a threshold filter to mask regions, segmenting them based on specified black and white threshold values. It's designed to isolate and enhance areas within the masks, making it easier to distinguish between different regions based on their intensity levels.
    - Inputs:
        - `masks` (Required): The input masks to be processed. These masks are segmented based on the provided threshold values, which determine the intensity levels that define the boundaries of the regions. Type should be `MASK`.
        - `black_threshold` (Required): The lower bound for pixel intensity. Pixels with intensity below this value are set to black, aiding in the segmentation of darker regions within the masks. Type should be `INT`.
        - `white_threshold` (Required): The upper bound for pixel intensity. Pixels with intensity above this value are set to white, aiding in the segmentation of lighter regions within the masks. Type should be `INT`.
    - Outputs:
        - `MASKS`: The output masks after applying the threshold filter, with regions segmented based on the specified black and white thresholds. Type should be `MASK`.
