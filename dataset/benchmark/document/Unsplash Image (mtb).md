- `Unsplash Image (mtb)`: The MTB_UnsplashImage node is designed to fetch and return an image from Unsplash based on specified dimensions and optional keywords. It utilizes the Unsplash API to dynamically source images, which can be tailored by the user through parameters such as image size and thematic keywords.
    - Inputs:
        - `width` (Required): Specifies the desired width of the image to be fetched. This dimension directly influences the resolution of the returned image, impacting its clarity and detail. Type should be `INT`.
        - `height` (Required): Determines the height of the image to be fetched. Similar to width, this parameter affects the resolution and aspect ratio of the resulting image. Type should be `INT`.
        - `random_seed` (Required): A seed value to introduce randomness in the image selection process, ensuring that requests for images are not deterministic and can vary with each call. Type should be `INT`.
        - `keyword` (Optional): An optional parameter that allows the user to specify a keyword to narrow down the image search, making the results more relevant to the desired theme or context. Type should be `STRING`.
    - Outputs:
        - `image`: The image retrieved from Unsplash, converted into a tensor format suitable for further processing or display within the node's operational context. Type should be `IMAGE`.
