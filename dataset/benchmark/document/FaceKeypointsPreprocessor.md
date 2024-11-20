- `FaceKeypointsPreprocessor`: The FaceKeypointsPreprocessor node is designed to preprocess images by extracting facial keypoints. This process involves analyzing the input image to detect faces and compute their keypoints, which are essential for various facial analysis tasks.
    - Inputs:
        - `faceanalysis` (Required): The 'faceanalysis' parameter is a model that has been loaded and prepared for face analysis. It is crucial for detecting faces within the image and extracting their keypoints, which are then used for further processing. Type should be `FACEANALYSIS`.
        - `image` (Required): The 'image' parameter represents the input image to be processed. It is analyzed by the face analysis model to detect faces and extract their keypoints, which are essential for the preprocessing task. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output is an image with facial keypoints extracted. This processed image is essential for tasks that require facial feature analysis, such as facial recognition or emotion detection. Type should be `IMAGE`.