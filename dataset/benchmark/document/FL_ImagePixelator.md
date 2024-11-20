- `FL_ImagePixelator`: The FL_ImagePixelator node applies pixelation effects to images, supporting both individual images and batches. It can process images represented as tensors or PIL images, applying a scale factor to pixelate the image and a kernel size for additional processing, enhancing the pixelation effect.
    - Inputs:
        - `image` (Required): The image to be pixelated. This can be a single image or a batch of images, in either torch.Tensor or PIL.Image format. It's the primary input for pixelation. Type should be `IMAGE`.
        - `scale_factor` (Required): Determines the intensity of the pixelation effect by scaling the image's resolution down before scaling it back up. Type should be `FLOAT`.
        - `kernel_size` (Required): Specifies the size of the kernel used in the additional processing step after pixelation, affecting the final appearance of the pixelated image. Type should be `INT`.
    - Outputs:
        - `image`: The pixelated image, processed according to the specified scale factor and kernel size. It can be a single image or a batch of images, in the same format as the input. Type should be `IMAGE`.