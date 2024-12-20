- `Image Compare (mtb)`: This node compares two images using different modes such as difference, blend, or checkerboard, and returns a new image highlighting the differences or combinations based on the selected mode.
    - Inputs:
        - `imageA` (Required): The first image to compare, represented as a torch.Tensor. It is one of the primary inputs for the comparison operation. Type should be `IMAGE`.
        - `imageB` (Required): The second image to compare, also represented as a torch.Tensor. This image is compared against the first to identify differences or create a blend/checkerboard effect. Type should be `IMAGE`.
        - `mode` (Required): A string indicating the comparison mode: 'checkerboard', 'diff', or 'blend'. The mode determines how the two images are compared and combined. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The resulting image after comparison, highlighting differences or combinations based on the selected mode. Type should be `IMAGE`.
