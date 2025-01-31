- `CompositeNoise __Inspire`: The CompositeNoise node in the Inspire pack is designed to enhance the generation process by applying a composite noise strategy. It integrates various noise manipulation techniques to adjust and refine the generated outputs, aiming to improve the quality and diversity of the results. This node likely combines different types of noise and processing methods to achieve a more nuanced and controlled generation outcome, making it a versatile tool for creative and generative tasks.
    - Inputs:
        - `destination` (Required): Specifies the destination for the noise application, indicating where the noise will be integrated within the generation process. Type should be `NOISE`.
        - `source` (Required): Identifies the source of the noise, which could be an external input or generated within the system, providing the basis for noise manipulation. Type should be `NOISE`.
        - `mode` (Required): Determines the mode of noise application, such as additive or multiplicative, affecting how the noise interacts with the generation process. Type should be `COMBO[STRING]`.
        - `x` (Required): Represents a specific parameter or variable related to the noise application, potentially influencing the direction or intensity of the noise. Type should be `INT`.
        - `y` (Required): Another parameter or variable that may affect the noise application process, offering additional control over the manipulation. Type should be `INT`.
    - Outputs:
        - `noise`: The generated or modified noise after application, showcasing the effects of the composite noise manipulation strategies. Type should be `NOISE`.
