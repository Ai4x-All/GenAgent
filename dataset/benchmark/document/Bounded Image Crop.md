- `Bounded Image Crop`: This node is designed to crop images based on specified bounding coordinates, ensuring that the cropping process is adapted to the dimensions of each image in a batch. It facilitates the precise extraction of image regions, allowing for focused analysis or manipulation of specific areas within images.
    - Inputs:
        - `image` (Required): The 'image' parameter represents the input image or a batch of images to be cropped. It plays a crucial role in determining the regions to be extracted based on the provided bounding coordinates. Type should be `IMAGE`.
        - `image_bounds` (Required): The 'image_bounds' parameter specifies the coordinates for cropping the image(s). It defines the rectangular region(s) within the image(s) to be extracted, ensuring targeted manipulation of the image content. Type should be `IMAGE_BOUNDS`.
    - Outputs:
        - `image`: The output is a cropped version of the input image or images, adjusted according to the specified bounding coordinates. It enables focused analysis or manipulation of specific regions within the images. Type should be `IMAGE`.
