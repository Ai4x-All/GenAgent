- `ToBinaryMask`: The ToBinaryMask node is designed to convert a given mask into a binary mask based on a specified threshold. This operation is fundamental in image processing tasks where binary masks are required to distinguish between areas of interest and the background.
    - Inputs:
        - `mask` (Required): The mask input represents the original mask that will be converted into a binary format. The conversion is based on the threshold value, making this input crucial for the operation's outcome. Type should be `MASK`.
        - `threshold` (Required): The threshold input determines the cutoff value for converting the original mask into a binary mask. Pixels with values above this threshold will be considered as part of the mask, affecting the binary mask's final appearance. Type should be `INT`.
    - Outputs:
        - `mask`: The output is a binary mask where each pixel is either 0 or 1, indicating whether it belongs to the mask or the background, respectively. Type should be `MASK`.