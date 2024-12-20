- `SaltMaskSubtract`: This node is designed to perform subtraction between two sets of masks, effectively computing the difference to highlight or remove specific regions within the masks.
    - Inputs:
        - `masks_a` (Required): The first set of masks to be subtracted from. This input plays a crucial role in determining the base for the subtraction operation. Type should be `MASK`.
        - `masks_b` (Required): The second set of masks to subtract from the first set. This input is essential for identifying the regions to be removed or highlighted in the resulting masks. Type should be `MASK`.
    - Outputs:
        - `MASKS`: The result of subtracting the second set of masks from the first, producing a new set of masks that highlight differences. Type should be `MASK`.
