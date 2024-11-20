- `FeatherMask`: The FeatherMask node applies a feathering effect to the edges of a given mask, smoothly transitioning the mask's edges by adjusting their opacity based on specified distances from each edge. This creates a softer, more blended edge effect.
    - Inputs:
        - `mask` (Required): The mask to which the feathering effect will be applied. It determines the area of the image that will be affected by the feathering. Type should be `MASK`.
        - `left` (Required): Specifies the distance from the left edge within which the feathering effect will be applied. Type should be `INT`.
        - `top` (Required): Specifies the distance from the top edge within which the feathering effect will be applied. Type should be `INT`.
        - `right` (Required): Specifies the distance from the right edge within which the feathering effect will be applied. Type should be `INT`.
        - `bottom` (Required): Specifies the distance from the bottom edge within which the feathering effect will be applied. Type should be `INT`.
    - Outputs:
        - `mask`: The output is a modified version of the input mask with a feathering effect applied to its edges. Type should be `MASK`.