- `SeargeEnablerInputs`: The SeargeEnablerInputs node is designed to process and validate the state of a given parameter, ensuring it aligns with predefined states within the system. It serves as a mechanism to enable or disable certain functionalities based on the state's value.
    - Inputs:
        - `state` (Required): Specifies the current state of a parameter, which determines the activation status of certain functionalities within the system. The default state is the second item in the predefined states list. Type should be `COMBO[STRING]`.
    - Outputs:
        - `state`: Returns the validated state of the parameter, which is used to control the activation of specific functionalities. Type should be `ENABLE_STATE`.
