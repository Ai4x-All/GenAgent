- `ADE_ReplaceOriginalPoseAspectRatio`: This node is designed to adjust the aspect ratio of original poses within the AnimateDiff framework, specifically for camera control applications. It modifies the dimensions of poses to match a new aspect ratio, ensuring that animations and visual effects are accurately rendered according to the desired spatial dimensions.
    - Inputs:
        - `poses` (Required): The list of poses to be adjusted. Each pose is a list of floats representing the spatial and rotational parameters of a camera control point. Type should be `CAMERACTRL_POSES`.
        - `orig_pose_width` (Required): The original width of the pose, which will be used to calculate the new aspect ratio. Type should be `INT`.
        - `orig_pose_height` (Required): The original height of the pose, which will be used to calculate the new aspect ratio. Type should be `INT`.
    - Outputs:
        - `cameractrl_poses`: The adjusted poses with the new aspect ratio applied, ready for further processing or animation within the AnimateDiff framework. Type should be `CAMERACTRL_POSES`.