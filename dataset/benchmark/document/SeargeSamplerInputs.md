- `SeargeSamplerInputs`: The SeargeSamplerInputs node is designed to manage and provide sampler and scheduler configurations for sampling processes. It abstracts the complexity of selecting appropriate sampling strategies by offering predefined options and defaults, thereby facilitating the customization and optimization of sampling operations.
    - Inputs:
        - `sampler_name` (Required): Specifies the name of the sampler to be used. This parameter allows for the selection among various predefined samplers, influencing the sampling behavior and results. Type should be `COMBO[STRING]`.
        - `scheduler` (Required): Determines the scheduling strategy to be employed during sampling. This parameter influences how samples are generated over time, affecting the overall sampling process. Type should be `COMBO[STRING]`.
    - Outputs:
        - `sampler_name`: The name of the selected sampler, reflecting the choice made for the sampling process. Type should be `SAMPLER_NAME`.
        - `scheduler`: The name of the chosen scheduler, indicating the scheduling strategy employed for sampling. Type should be `SCHEDULER_NAME`.