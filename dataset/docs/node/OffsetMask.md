- `OffsetMask`: The OffsetMask node is designed to manipulate and transform masks by applying specified offsets, rotations, and duplication factors. It enables the creation of multiple variations of a given mask, allowing for dynamic adjustments in positioning and orientation, which can be particularly useful in image processing and augmentation tasks.
    - Parameters:
        - `x`: Specifies the horizontal offset to apply to the mask. This parameter controls the lateral displacement of the mask. Type should be `INT`.
        - `y`: Specifies the vertical offset to apply to the mask. This parameter controls the vertical displacement of the mask. Type should be `INT`.
        - `angle`: Defines the angle in degrees for rotating the mask. This parameter allows for the rotational adjustment of the mask. Type should be `INT`.
        - `duplication_factor`: The number of times the mask is duplicated to form a batch. This parameter enables the creation of multiple mask variations from a single input. Type should be `INT`.
        - `roll`: Determines whether edge wrapping is applied during the offset. This boolean parameter influences how the mask is manipulated at its borders. Type should be `BOOLEAN`.
        - `incremental`: Indicates whether the offset should be applied incrementally. This boolean parameter affects the method of mask transformation. Type should be `BOOLEAN`.
        - `padding_mode`: Specifies the padding mode to be used when transforming the mask. This parameter affects how the mask's edges are handled during the offset. Type should be `COMBO[STRING]`.
    - Inputs:
        - `mask`: The input mask or batch of masks to be transformed. This parameter is central to the node's operation, serving as the basis for all subsequent transformations. Type should be `MASK`.
    - Outputs:
        - `mask`: The transformed mask or batch of masks after applying the specified offsets, rotations, and duplication factors. Type should be `MASK`.