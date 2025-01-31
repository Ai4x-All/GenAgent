- `CLIPSeg Batch Masking`: This node applies the CLIPSeg model to a batch of images, generating corresponding segmentation masks based on the provided text descriptions. It leverages the CLIPSeg model's ability to understand the content of images in relation to textual descriptions, producing masks that highlight areas of interest specified by the text.
    - Inputs:
        - `image_a` (Required): The first input image tensor to be segmented. It serves as the primary visual context for the segmentation process. Type should be `IMAGE`.
        - `image_b` (Required): The second input image tensor to be segmented. It acts as an additional visual context for the segmentation process. Type should be `IMAGE`.
        - `text_a` (Required): The first textual description that specifies the content to be segmented within the images. It guides the CLIPSeg model in focusing on relevant parts of the images for mask generation. Type should be `STRING`.
        - `text_b` (Required): The second textual description that specifies the content to be segmented within the images. It provides additional guidance to the CLIPSeg model for mask generation. Type should be `STRING`.
        - `image_c` (Optional): An optional third input image tensor to be segmented, providing further visual context if available. Type should be `IMAGE`.
        - `image_d` (Optional): An optional fourth input image tensor to be segmented, providing further visual context if available. Type should be `IMAGE`.
        - `image_e` (Optional): An optional fifth input image tensor to be segmented, providing further visual context if available. Type should be `IMAGE`.
        - `image_f` (Optional): An optional sixth input image tensor to be segmented, providing further visual context if available. Type should be `IMAGE`.
        - `text_c` (Optional): An optional third textual description, offering additional content specification for segmentation. Type should be `STRING`.
        - `text_d` (Optional): An optional fourth textual description, offering additional content specification for segmentation. Type should be `STRING`.
        - `text_e` (Optional): An optional fifth textual description, offering additional content specification for segmentation. Type should be `STRING`.
        - `text_f` (Optional): An optional sixth textual description, offering additional content specification for segmentation. Type should be `STRING`.
    - Outputs:
        - `IMAGES_BATCH`: A batch of original images processed through the node. Type should be `IMAGE`.
        - `MASKS_BATCH`: A batch of segmentation masks corresponding to the input images and text descriptions. Type should be `MASK`.
        - `MASK_IMAGES_BATCH`: A batch of inverted mask images derived from the segmentation masks. Type should be `IMAGE`.
