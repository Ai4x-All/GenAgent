- `CLAHE`: The CLAHE node applies the Contrast Limited Adaptive Histogram Equalization algorithm to enhance the contrast of images. It adjusts image intensities to enhance the contrast locally, taking into account specific parameters like clip limit and tile grid size for finer control over the process.
    - Parameters:
        - `clip_limit`: Defines the threshold for contrast limiting. This parameter helps in controlling the enhancement of contrast, preventing it from amplifying noise in relatively homogeneous regions of the image. Type should be `INT`.
        - `tile_grid_x`: Specifies the number of tiles in the horizontal direction for dividing the image. It determines the granularity of the contrast enhancement process. Type should be `INT`.
        - `tile_grid_y`: Specifies the number of tiles in the vertical direction for dividing the image. Similar to tile_grid_x, it affects the granularity of the contrast enhancement. Type should be `INT`.
    - Inputs:
        - `src`: The source image to be processed. It serves as the input on which the CLAHE algorithm is applied to enhance local contrast. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output image after applying CLAHE. It is the enhanced version of the input image with improved local contrast. Type should be `IMAGE`.