- `UpperBodyTrackingFromPoseKps`: This node is designed to process pose keypoints for upper body tracking, extracting and formatting specific body parts such as the torso, arms, and face from pose detection results. It enhances the keypoints data by appending additional points for completeness and accuracy, particularly for facial features, and compiles the results into structured pose results for further analysis or visualization.
    - Inputs:
        - `pose_kps` (Required): The input pose keypoints, which are essential for identifying and tracking the upper body parts in images or video frames. This data includes body, hands, and face keypoints along with their scores. Type should be `POSE_KEYPOINT`.
        - `id_include` (Required): An optional string to include specific IDs in the tracking process, allowing for targeted analysis of pose keypoints. Type should be `STRING`.
        - `Head_width_height` (Required): Specifies the width and height for the head part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `Neck_width_height` (Required): Specifies the width and height for the neck part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `Shoulder_width_height` (Required): Specifies the width and height for the shoulder part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `Torso_width_height` (Required): Specifies the width and height for the torso part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `RArm_width_height` (Required): Specifies the width and height for the right arm part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `RForearm_width_height` (Required): Specifies the width and height for the right forearm part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `LArm_width_height` (Required): Specifies the width and height for the left arm part, used in calculating dimensions for tracking. Type should be `STRING`.
        - `LForearm_width_height` (Required): Specifies the width and height for the left forearm part, used in calculating dimensions for tracking. Type should be `STRING`.
    - Outputs:
        - `tracking`: Structured data representing the tracking of upper body parts, including detailed information about body keypoints, hands, and face, along with their respective scores. Type should be `TRACKING`.
        - `prompt`: A textual prompt or summary generated based on the tracking results, providing insights or conclusions from the analysis. Type should be `STRING`.
