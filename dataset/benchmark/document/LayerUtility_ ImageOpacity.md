- `LayerUtility_ ImageOpacity`: The ImageOpacity node is designed to adjust the opacity of an image, optionally applying an inversion mask to selectively modify the transparency across the image. It provides a way to dynamically control the visual appearance of images by altering their transparency levels.
    - Inputs:
        - `image` (Required): The 'image' parameter represents the input image to which the opacity adjustment will be applied. It is essential for defining the base visual content that will undergo transparency modification. Type should be `IMAGE`.
        - `opacity` (Required): The 'opacity' parameter specifies the degree of transparency to apply to the image, with a range from 0 (completely transparent) to 100 (fully opaque). It allows for fine-tuning the visibility of the image. Type should be `INT`.
        - `invert_mask` (Required): The 'invert_mask' parameter determines whether to invert the mask applied to the image, enabling selective opacity adjustments across different regions of the image. Type should be `BOOLEAN`.
        - `mask` (Optional): The 'mask' parameter, when provided, specifies a mask to apply to the image for targeted opacity adjustments. It is optional and used for more complex transparency effects. Type should be `MASK`.
    - Outputs:
        - `image`: The modified image with adjusted opacity. Type should be `IMAGE`.
        - `mask`: The mask used for opacity adjustment, if any was applied. Type should be `MASK`.