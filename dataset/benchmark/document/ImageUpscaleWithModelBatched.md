- `ImageUpscaleWithModelBatched`: This node is designed to upscale images using a specified model, with the added functionality of processing images in sub-batches. This approach helps in managing VRAM usage more efficiently, making it suitable for systems with limited memory resources.
    - Inputs:
        - `upscale_model` (Required): The model used for upscaling images. It determines the quality and characteristics of the output images. Type should be `UPSCALE_MODEL`.
        - `images` (Required): The batch of images to be upscaled. This input allows the node to process multiple images simultaneously, optimizing throughput. Type should be `IMAGE`.
        - `per_batch` (Required): Defines the number of images to process in each sub-batch. This parameter helps in controlling VRAM usage by breaking down the batch into smaller, manageable chunks. Type should be `INT`.
    - Outputs:
        - `image`: The upscaled images, returned as a batch. This output provides higher resolution versions of the input images. Type should be `IMAGE`.