- `ImpactSimpleDetectorSEGSPipe`: This node is designed to perform detection tasks on images, utilizing segmentation models to identify and process specific features or objects within those images. It abstracts the complexity of segmentation and detection algorithms, providing a straightforward interface for segmenting images and detecting objects or features based on specified criteria.
    - Inputs:
        - `detailer_pipe` (Required): Specifies the pipeline for detailing the detection process, enhancing the precision of detected segments. Type should be `DETAILER_PIPE`.
        - `image` (Required): The input image to be processed for segmentation and detection. Type should be `IMAGE`.
        - `bbox_threshold` (Required): The threshold value for bounding box detection, controlling the sensitivity of the detection process. Type should be `FLOAT`.
        - `bbox_dilation` (Required): Determines the dilation level of bounding boxes, affecting the size and coverage of detected segments. Type should be `INT`.
        - `crop_factor` (Required): Controls the cropping factor for the detected segments, influencing the area around the detected features that is included in the output. Type should be `FLOAT`.
        - `drop_size` (Required): Specifies the minimum size for detected segments, filtering out smaller detections. Type should be `INT`.
        - `sub_threshold` (Required): The threshold for sub-segment detection, refining the detection process within the already detected segments. Type should be `FLOAT`.
        - `sub_dilation` (Required): Determines the dilation level for sub-segments, adjusting the coverage within detected segments. Type should be `INT`.
        - `sub_bbox_expansion` (Required): Controls the expansion of bounding boxes for sub-segments, affecting the area covered by each sub-segment detection. Type should be `INT`.
        - `sam_mask_hint_threshold` (Required): The threshold for mask hinting in SAM models, influencing the selection of segments based on their relevance to the SAM model's criteria. Type should be `FLOAT`.
        - `post_dilation` (Optional): unknown Type should be `INT`.
    - Outputs:
        - `segs`: Produces segmented parts of the image based on the detection criteria, including detailed information about each segment. Type should be `SEGS`.
