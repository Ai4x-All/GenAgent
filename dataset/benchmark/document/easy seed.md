- `easy seed`: The `easy seed` node is designed to manage and control the seed value used in generation processes, allowing for the replication of results or the introduction of variability. It supports operations such as setting a fixed seed, incrementing, decrementing, or randomizing the seed for each node or globally across the workflow.
    - Inputs:
        - `seed` (Required): The initial seed value, which serves as the basis for generation processes. It determines the starting point for any pseudo-random operations, affecting the reproducibility and variation of outputs. Type should be `INT`.
    - Outputs:
        - `seed`: The seed value after being processed according to the specified action. This allows for controlled variation or consistency in generation processes. Type should be `INT`.
