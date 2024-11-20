- `Seed Generator`: The Seed Generator node is designed to provide a deterministic or randomized seed value for various operations within the image saving process. It ensures that operations can be repeatable with a fixed seed or varied with a random seed, supporting both consistency and diversity in output.
    - Inputs:
        - `seed` (Required): The seed parameter allows users to specify a seed value for generating deterministic outputs. If not provided, a default value is used, ensuring repeatability or randomness in operations. Type should be `INT`.
    - Outputs:
        - `int`: Outputs an integer representing the seed value, which can be used to initialize random number generators or other processes requiring a seed. Type should be `INT`.