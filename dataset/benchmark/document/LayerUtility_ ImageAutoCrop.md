- `LayerUtility_ ImageAutoCrop`: The ImageAutoCrop node is designed to automatically crop images based on certain criteria, such as the presence of a mask or specific image features. It aims to streamline the process of refining image layers by removing unnecessary or undesired parts, enhancing the focus and composition of the image.
    - Inputs:
        - `image` (Required): Represents the input image to be auto-cropped. It is crucial for determining the area of interest and executing the crop operation. Type should be `IMAGE`.
        - `background_color` (Required): Specifies the background color to be used in the cropping process, particularly when adjusting the image to a new aspect ratio or filling in areas after cropping. Type should be `STRING`.
        - `aspect_ratio` (Required): Defines the desired aspect ratio for the cropped image, which can be set to custom values, original, or based on the detection of a mask. Type should be `COMBO[STRING]`.
        - `proportional_width` (Required): When using a custom aspect ratio, this value specifies the width proportion to calculate the new aspect ratio. Type should be `INT`.
        - `proportional_height` (Required): When using a custom aspect ratio, this value specifies the height proportion to calculate the new aspect ratio. Type should be `INT`.
        - `scale_to_longest_side` (Required): A boolean indicating whether to scale the image based on the longest side, maintaining the aspect ratio. Type should be `BOOLEAN`.
        - `longest_side` (Required): Specifies the target length of the longest side of the image when scaling is applied. Type should be `INT`.
        - `detect` (Required): Determines the method used to detect the cropping area, such as minimum bounding rectangle, maximum inscribed rectangle, or mask area detection. Type should be `COMBO[STRING]`.
        - `border_reserve` (Required): The amount of border to reserve around the detected cropping area, adding space around the crop. Type should be `INT`.
        - `ultra_detail_range` (Required): Specifies the range for enhancing detail around the edges of the mask, used in conjunction with certain matting methods. Type should be `INT`.
        - `matting_method` (Required): The method used for generating a mask around the subject of the image, such as 'SegmentAnything' or a simple background removal. Type should be `COMBO[STRING]`.
        - `sam_model` (Required): Specifies the model used for the 'SegmentAnything' matting method, affecting the quality and accuracy of the generated mask. Type should be `COMBO[STRING]`.
        - `grounding_dino_model` (Required): Specifies the DINO model used for grounding the segmentation, enhancing the mask's accuracy around the subject. Type should be `COMBO[STRING]`.
        - `sam_threshold` (Required): The threshold value for the SAM model, determining the sensitivity of the segmentation process. Type should be `FLOAT`.
        - `sam_prompt` (Required): The prompt used with the SAM model to guide the segmentation process, influencing the areas of focus. Type should be `STRING`.
    - Outputs:
        - `cropped_image`: The result of the auto-cropping process, which is a refined version of the original image with unnecessary parts removed. Type should be `IMAGE`.
        - `box_preview`: A visual representation of the cropping box applied to the original image, useful for previewing the crop area before finalization. Type should be `IMAGE`.
        - `cropped_mask`: The corresponding mask of the cropped image, adjusted to match the new dimensions and area of the cropped image. Type should be `MASK`.