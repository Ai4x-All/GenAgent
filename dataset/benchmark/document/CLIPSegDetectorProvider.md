- `CLIPSegDetectorProvider`: The CLIPSegDetectorProvider node is designed to leverage the capabilities of CLIPSeg for object detection within images. It processes textual descriptions and image characteristics to identify and delineate objects, utilizing parameters such as blur, threshold, and dilation factor to refine the detection process.
    - Inputs:
        - `text` (Required): The textual description of the object to be detected. This parameter is crucial for guiding the CLIPSeg model in identifying the relevant objects within the image. Type should be `STRING`.
        - `blur` (Required): Specifies the level of blur applied to the image before detection. This can help in reducing noise and improving the accuracy of object detection. Type should be `FLOAT`.
        - `threshold` (Required): A threshold value that determines the sensitivity of object detection. Higher values may result in fewer detections, while lower values can increase the detection of minor features. Type should be `FLOAT`.
        - `dilation_factor` (Required): Determines the extent to which the detected object's boundaries are expanded or contracted. This can be useful in adjusting the preciseness of the object's outline. Type should be `INT`.
    - Outputs:
        - `bbox_detector`: Provides an object detector based on the CLIPSeg model, capable of identifying and bounding objects within images based on textual descriptions. Type should be `BBOX_DETECTOR`.
