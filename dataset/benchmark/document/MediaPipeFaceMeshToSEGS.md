- `MediaPipeFaceMeshToSEGS`: The MediaPipeFaceMeshToSEGS node transforms facial landmarks detected by MediaPipe's FaceMesh into a structured format suitable for SEGS (Segmentation and Geometry Schema), enabling further manipulation and analysis of facial features within the SEGS framework.
    - Inputs:
        - `image` (Required): The input image on which facial landmark detection is performed. It serves as the basis for generating the SEGS representation of facial features. Type should be `IMAGE`.
        - `crop_factor` (Required): Determines the extent to which the detected facial region is cropped. A higher value results in a tighter crop around the facial landmarks, affecting the final SEGS output. Type should be `FLOAT`.
        - `bbox_fill` (Required): Specifies how the bounding box around detected facial landmarks is filled, influencing the appearance and structure of the resulting SEGS. Type should be `BOOLEAN`.
        - `crop_min_size` (Required): Sets the minimum size for the cropped facial region, ensuring that the output SEGS does not fall below a certain spatial resolution. Type should be `INT`.
        - `drop_size` (Required): Defines the threshold below which detected facial regions are disregarded, preventing the generation of SEGS for insignificantly small facial features. Type should be `INT`.
        - `dilation` (Required): Applies a dilation operation to the facial landmarks' bounding box, expanding its size and potentially including additional context in the SEGS output. Type should be `INT`.
        - `face` (Required): Indicates whether the face region should be included in the SEGS output, allowing for specific facial feature analysis. Type should be `BOOLEAN`.
        - `mouth` (Required): Determines whether the mouth region is included in the SEGS, enabling detailed examination and manipulation of this specific area. Type should be `BOOLEAN`.
        - `left_eyebrow` (Required): Specifies the inclusion of the left eyebrow in the SEGS output, facilitating focused analysis on this facial feature. Type should be `BOOLEAN`.
        - `left_eye` (Required): Controls the inclusion of the left eye in the SEGS, allowing for targeted manipulation and study of eye-related aspects. Type should be `BOOLEAN`.
        - `left_pupil` (Required): Determines the inclusion of the left pupil in the SEGS, enabling precise analysis and adjustments to this specific part of the eye. Type should be `BOOLEAN`.
        - `right_eyebrow` (Required): Specifies the inclusion of the right eyebrow in the SEGS output, facilitating focused analysis on this facial feature. Type should be `BOOLEAN`.
        - `right_eye` (Required): Controls the inclusion of the right eye in the SEGS, allowing for targeted manipulation and study of eye-related aspects. Type should be `BOOLEAN`.
        - `right_pupil` (Required): Determines the inclusion of the right pupil in the SEGS, enabling precise analysis and adjustments to this specific part of the eye. Type should be `BOOLEAN`.
    - Outputs:
        - `segs`: The output is a structured SEGS representation of the detected facial landmarks, ready for further processing and analysis within the SEGS framework. Type should be `SEGS`.
