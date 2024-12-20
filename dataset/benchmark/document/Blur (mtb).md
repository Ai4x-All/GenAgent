- `Blur (mtb)`: The Blur node applies a Gaussian blur to an image, allowing for both uniform and variable blurring across the image. This process can be used to reduce image noise and detail, simulating the effect of shooting in a lower resolution or with a softer focus lens.
    - Inputs:
        - `image` (Required): The input image to be blurred. This is the primary data upon which the blur effect is applied, serving as the foundation for the operation. Type should be `IMAGE`.
        - `sigmaX` (Required): Specifies the standard deviation in the x-direction for the Gaussian kernel. This parameter controls the amount of blur horizontally. Type should be `FLOAT`.
        - `sigmaY` (Required): Specifies the standard deviation in the y-direction for the Gaussian kernel. This parameter controls the amount of blur vertically. Type should be `FLOAT`.
        - `sigmasX` (Optional): An optional list of standard deviations in the x-direction for applying variable blur across different parts of the image. Type should be `FLOATS`.
        - `sigmasY` (Optional): An optional list of standard deviations in the y-direction for applying variable blur across different parts of the image. Type should be `FLOATS`.
    - Outputs:
        - `image`: The output image after applying the Gaussian blur. This image will have reduced noise and detail, with a softer appearance. Type should be `IMAGE`.
