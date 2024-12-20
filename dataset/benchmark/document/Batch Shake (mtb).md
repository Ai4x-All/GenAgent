- `Batch Shake (mtb)`: The Batch Shake node applies a dynamic shaking effect to a batch of images, utilizing parameters such as position, rotation, and frequency to simulate motion or instability effects.
    - Inputs:
        - `images` (Required): The batch of images to be processed. This input is crucial for defining the visual content that will undergo the shaking effect. Type should be `IMAGE`.
        - `position_amount_x` (Required): Determines the horizontal intensity of the shaking effect, affecting how far images can move along the x-axis. Type should be `FLOAT`.
        - `position_amount_y` (Required): Determines the vertical intensity of the shaking effect, affecting how far images can move along the y-axis. Type should be `FLOAT`.
        - `rotation_amount` (Required): Controls the amount of rotation applied to the images, simulating a twisting motion. Type should be `FLOAT`.
        - `frequency` (Required): Defines the frequency of the shaking effect, influencing the speed of motion changes. Type should be `FLOAT`.
        - `frequency_divider` (Required): Modifies the base frequency, allowing for finer control over the shaking effect's speed. Type should be `FLOAT`.
        - `octaves` (Required): Adjusts the complexity of the shaking pattern, adding layers of motion for a more nuanced effect. Type should be `INT`.
        - `seed` (Required): Sets the initial seed for random number generation, ensuring reproducible shaking patterns. Type should be `INT`.
    - Outputs:
        - `image`: The processed image after applying the shaking effect. Type should be `IMAGE`.
        - `pos_x`: The horizontal translation values applied to each image in the batch. Type should be `FLOATS`.
        - `pos_y`: The vertical translation values applied to each image in the batch. Type should be `FLOATS`.
        - `rot`: The rotation values applied to each image in the batch, reflecting the degree of twist. Type should be `FLOATS`.
