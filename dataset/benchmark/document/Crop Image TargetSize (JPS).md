- `Crop Image TargetSize (JPS)`: The Crop Image TargetSize node is designed for adjusting images to specific target dimensions with options for cropping, zooming, and applying various interpolation and sharpening techniques. It provides flexibility in image processing by allowing for precise control over the dimensions and quality of the output image, catering to different requirements for image manipulation.
    - Inputs:
        - `image` (Required): The input image to be processed. It serves as the base for cropping, resizing, and applying other transformations to meet the target dimensions and quality specifications. Type should be `IMAGE`.
        - `target_w` (Required): The target width for the output image. This parameter dictates the desired width that the image should be adjusted to, either by cropping or resizing. Type should be `INT`.
        - `target_h` (Required): The target height for the output image. Similar to target_w, it specifies the desired height for the image adjustment. Type should be `INT`.
        - `crop_position` (Required): Specifies the position from which the image should be cropped. This affects how the image is aligned before cropping to the target dimensions. Type should be `COMBO[STRING]`.
        - `offset` (Required): A general offset value used when adjusting the image's position before cropping. It allows for fine-tuning the crop alignment. Type should be `INT`.
        - `interpolation` (Required): The method used for resizing the image. Different interpolation techniques can affect the image's quality and appearance. Type should be `COMBO[STRING]`.
        - `sharpening` (Required): Determines whether and how much the output image should be sharpened, enhancing its details and overall clarity. Type should be `FLOAT`.
    - Outputs:
        - `IMAGE`: The processed image after applying the specified cropping, zooming, interpolation, and sharpening transformations. It represents the final output that meets the target dimensions and quality criteria. Type should be `IMAGE`.