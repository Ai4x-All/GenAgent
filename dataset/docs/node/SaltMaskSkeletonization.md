- `SaltMaskSkeletonization`: The SaltMaskSkeletonization node is designed to transform input mask images into their skeletonized versions, effectively reducing the masks to their simplest form while preserving their overall geometry. This process is useful for applications requiring a minimal representation of shapes within the masks.
    - Parameters:
        - `iterations`: Specifies the number of times the erosion operation is applied to each mask, influencing the thinness of the resulting skeleton. Type should be `INT`.
        - `strength`: Determines the intensity of the skeletonization process, affecting the final skeletal structure's prominence. Type should be `INT`.
    - Inputs:
        - `masks`: The input masks to be skeletonized, where each mask represents a distinct region to be processed into its skeletal form. Type should be `MASK`.
    - Outputs:
        - `MASKS`: The output tensor containing the skeletonized versions of the input masks, with each skeleton representing the minimal structure of the original mask. Type should be `MASK`.