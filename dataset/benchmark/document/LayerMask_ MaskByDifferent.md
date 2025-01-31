- `LayerMask_ MaskByDifferent`: This node is designed to create a mask based on differences between two images, enabling the identification and isolation of unique elements. It facilitates dynamic segmentation by analyzing and contrasting the visual characteristics present in each layer.
    - Inputs:
        - `image_i` (Required): The first and second images to be compared, serving as reference points for identifying differences. These images are used to detect variations and unique features, enabling the creation of a mask that highlights these differences. Type should be `IMAGE`.
        - `gain` (Required): Adjusts the sensitivity of the difference detection, influencing the intensity of the identified changes. Type should be `FLOAT`.
        - `fix_gap` (Required): Defines the tolerance for gap fixing in the generated mask, helping to smooth and refine the mask's edges. Type should be `INT`.
        - `fix_threshold` (Required): Sets the threshold for fixing gaps within the mask, further enhancing mask accuracy by refining edge details. Type should be `FLOAT`.
        - `main_subject_detect` (Required): A boolean flag that, when enabled, focuses the difference detection on the main subject of the images, potentially improving the relevance of the generated mask. Type should be `BOOLEAN`.
    - Outputs:
        - `mask`: The resulting mask that highlights the differences between the two input images, isolating unique elements and features. Type should be `MASK`.
