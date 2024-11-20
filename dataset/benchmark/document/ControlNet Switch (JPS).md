- `ControlNet Switch (JPS)`: The ControlNet Switch node is designed to dynamically select between multiple control network configurations based on a given selection input. It facilitates the flexible manipulation of control networks within a processing pipeline, allowing for the conditional application of different control network settings.
    - Inputs:
        - `select` (Required): Specifies the index of the control network to be selected for output. This input determines which control network configuration is applied, enabling dynamic switching between configurations. Type should be `INT`.
        - `ctrlnet_i` (Optional): Represents a generic control network configuration option, where 'i' can range from 1 to 5, indicating the selectable control network configurations based on the 'select' input. Type should be `CONTROL_NET`.
    - Outputs:
        - `ctrlnet_out`: Outputs the selected control network configuration, facilitating its application in subsequent processing steps. Type should be `CONTROL_NET`.