- `ImpactScaleBy_BBOX_SEG_ELT`: This node scales the bounding box of a segmentation element by a specified factor, adjusting the segmentation mask accordingly. It ensures that the scaled bounding box and its corresponding mask are correctly aligned and sized, maintaining the integrity of the segmentation element.
    - Parameters:
        - `scale_by`: The factor by which the bounding box is to be scaled. This directly influences the size of the resulting bounding box and its associated mask. Type should be `FLOAT`.
    - Inputs:
        - `seg`: The segmentation element whose bounding box is to be scaled. It is crucial for determining the area of interest within the image. Type should be `SEG_ELT`.
    - Outputs:
        - `seg_elt`: The scaled segmentation element, including the adjusted bounding box and mask. Type should be `SEG_ELT`.