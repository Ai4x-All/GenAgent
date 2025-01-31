- `LayerMask_ PersonMaskUltra V2`: This node specializes in generating a precise mask for individuals within an image, leveraging advanced segmentation techniques to accurately distinguish human figures from the background. It's designed to enhance image processing tasks by providing a detailed layer mask for person segmentation.
    - Inputs:
        - `images` (Required): The input images for which the person mask will be generated, serving as the primary data for segmentation. Type should be `IMAGE`.
        - `face` (Required): A boolean flag to include or exclude the face in the person mask, affecting the segmentation focus. Type should be `BOOLEAN`.
        - `hair` (Required): A boolean flag to include or exclude hair in the person mask, influencing the mask's detail level. Type should be `BOOLEAN`.
        - `body` (Required): A boolean flag to include or exclude the body in the person mask, impacting the overall segmentation. Type should be `BOOLEAN`.
        - `clothes` (Required): A boolean flag to include or exclude clothes in the person mask, modifying the mask's coverage. Type should be `BOOLEAN`.
        - `accessories` (Required): A boolean flag to include or exclude accessories in the person mask, altering the segmentation details. Type should be `BOOLEAN`.
        - `background` (Required): A boolean flag to include or exclude the background in the person mask, affecting the mask's clarity. Type should be `BOOLEAN`.
        - `confidence` (Required): Sets the confidence level for the segmentation, influencing the precision of the person mask. Type should be `FLOAT`.
        - `detail_method` (Required): Specifies the method used for enhancing the detail in the mask, affecting the mask's accuracy and quality. Type should be `COMBO[STRING]`.
        - `detail_erode` (Required): Determines the extent of erosion applied to the mask's details, influencing the mask's edge sharpness. Type should be `INT`.
        - `detail_dilate` (Required): Determines the extent of dilation applied to the mask's details, affecting the mask's edge softness. Type should be `INT`.
        - `black_point` (Required): unknown Type should be `FLOAT`.
        - `white_point` (Required): unknown Type should be `FLOAT`.
        - `process_detail` (Required): unknown Type should be `BOOLEAN`.
        - `device` (Required): Specifies the computing device (CPU or GPU) used for processing, affecting the node's performance. Type should be `COMBO[STRING]`.
        - `max_megapixels` (Required): Limits the maximum size of the images processed, balancing detail and processing time. Type should be `FLOAT`.
    - Outputs:
        - `image`: The original image overlaid with the generated mask, showcasing the segmentation result. Type should be `IMAGE`.
        - `mask`: The generated mask that accurately outlines human figures within the image, ready for further image processing applications. Type should be `MASK`.
