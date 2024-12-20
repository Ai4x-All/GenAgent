- `ImpactConcatConditionings`: The ImpactConcatConditionings node is designed to concatenate multiple conditioning inputs into a single conditioning output. This process is essential for combining various conditioning elements to enhance or specify the generation process further.
    - Inputs:
        - `conditioning1` (Required): The primary conditioning input. This input serves as the base to which additional conditionings are concatenated, influencing the overall output by combining multiple conditioning aspects. Type should be `CONDITIONING`.
    - Outputs:
        - `conditioning`: The concatenated conditioning output, which combines the input conditionings into a unified form, enhancing the generation process. Type should be `CONDITIONING`.
