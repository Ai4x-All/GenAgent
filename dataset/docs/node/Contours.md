- `Contours`: The `Contours` node is designed to identify and extract contours from an image based on specified retrieval and approximation modes. It transforms the input image into a grayscale version, applies thresholding if necessary, and utilizes OpenCV's contour finding capabilities to return the identified contours along with their hierarchy.
    - Parameters:
        - `retrieval_mode`: Specifies the contour retrieval mode, which determines how the contours are organized or retrieved. This choice impacts the structure of the output contours, affecting how they are hierarchically related or grouped. Type should be `COMBO[STRING]`.
        - `approximation_mode`: Defines the method used to approximate the contours. Different modes can simplify the contour shapes in various ways, affecting the level of detail and the overall shape of the extracted contours. Type should be `COMBO[STRING]`.
    - Inputs:
        - `image`: The input image from which contours are to be extracted. This image is crucial as it serves as the basis for contour detection, directly influencing the contours that are identified and their characteristics. Type should be `IMAGE`.
    - Outputs:
        - `cv_contours`: A list of detected contours in the image, representing the primary output of contour detection. Type should be `CV_CONTOURS`.
        - `cv_contour`: A single contour selected from the list of detected contours, based on specific criteria or processing steps. Type should be `CV_CONTOUR`.
        - `cv_contours_hierarchy`: The hierarchical representation of contours, indicating the relationship between contour levels. This hierarchy provides insight into the nesting and organization of contours within the image. Type should be `CV_CONTOURS_HIERARCHY`.