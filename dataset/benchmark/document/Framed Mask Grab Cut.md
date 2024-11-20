- `Framed Mask Grab Cut`: The Framed Mask Grab Cut node is designed to apply the GrabCut algorithm with additional framing options to segment the foreground from the background in images. It allows for the specification of probable and sure foreground and background areas, and incorporates frame options to exclude certain margins from consideration, enhancing the flexibility and accuracy of the segmentation process.
    - Inputs:
        - `image` (Required): The input image on which the GrabCut algorithm will be applied. It serves as the primary data for foreground-background segmentation. Type should be `IMAGE`.
        - `thresh` (Required): A thresholded image indicating areas that might be the foreground or background. This parameter helps in refining the segmentation by marking uncertain areas. Type should be `IMAGE`.
        - `iterations` (Required): The number of iterations the GrabCut algorithm should run, affecting the refinement of the segmentation. Type should be `INT`.
        - `margin` (Required): Specifies the margin size to be excluded from the frame options, allowing for more precise control over the area considered for segmentation. Type should be `INT`.
        - `frame_option` (Required): Defines the frame options to apply, such as ignoring certain margins, to tailor the segmentation process to specific requirements. Type should be `COMBO[STRING]`.
        - `threshold_FGD` (Required): The threshold value used to classify pixels in 'thresh' image as foreground. Type should be `INT`.
        - `threshold_PR_FGD` (Required): The threshold value used to classify pixels in 'thresh' image as probable foreground. Type should be `INT`.
        - `output_format` (Required): The desired format for the output image, allowing for compatibility with different processing or display requirements. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The segmented image with the foreground isolated from the background, based on the GrabCut algorithm and additional framing options. Type should be `IMAGE`.