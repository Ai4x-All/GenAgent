- `MergeImageChannels`: The MergeImageChannels node is designed for combining separate image channels (red, green, and blue) into a single composite image. It optionally supports the inclusion of an alpha channel for transparency, allowing for more complex image compositions.
    - Inputs:
        - `red` (Required): The red channel of the image, which contributes to the overall color composition by defining the red intensity. Type should be `IMAGE`.
        - `green` (Required): The green channel of the image, which contributes to the overall color composition by defining the green intensity. Type should be `IMAGE`.
        - `blue` (Required): The blue channel of the image, which contributes to the overall color composition by defining the blue intensity. Type should be `IMAGE`.
        - `mask` (Optional): An optional alpha channel for adding transparency to the final image, enhancing its compositional complexity. Type should be `MASK`.
    - Outputs:
        - `image`: The resulting image after merging the red, green, and blue channels, optionally with an alpha channel for transparency. Type should be `IMAGE`.