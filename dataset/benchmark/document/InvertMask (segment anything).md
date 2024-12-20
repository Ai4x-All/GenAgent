- `InvertMask (segment anything)`: The InvertMask node is designed for the inversion of mask values, effectively flipping the masked and unmasked areas. This operation is fundamental in image processing tasks where the focus of interest needs to be switched between the foreground and background.
    - Inputs:
        - `mask` (Required): The 'mask' parameter represents the input mask whose values are to be inverted. This inversion process is crucial for tasks that require toggling the areas of interest within an image. Type should be `MASK`.
    - Outputs:
        - `mask`: The output is a mask with inverted values, where previously masked areas are now unmasked and vice versa, facilitating operations that require the opposite area of interest. Type should be `MASK`.
