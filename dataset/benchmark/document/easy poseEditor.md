- `easy poseEditor`: The `poseEditor` node is designed to facilitate the editing of poses within images. It provides a framework for adjusting and manipulating the positioning and orientation of subjects in an image, leveraging a set of predefined input types to customize the editing process.
    - Inputs:
        - `image` (Required): `image` is the primary input for the pose editing process, representing the image within which poses are to be edited or manipulated. It is essential for defining the starting point of the pose adjustment workflow. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The output `image` is the result of the pose editing process, showcasing the adjusted or manipulated poses within the original image context. Type should be `IMAGE`.