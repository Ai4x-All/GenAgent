- `CR Latent Input Switch`: The CR_LatentInputSwitch node is designed to switch between two latent inputs based on a specified condition. It facilitates dynamic workflow paths in generative models by allowing the selection of different latent representations.
    - Parameters:
        - `Input`: Determines which latent input to select. A value of 1 selects the first latent input, while a value of 2 selects the second. Type should be `INT`.
    - Inputs:
        - `latent1`: The first latent input option. This input is selected if the 'Input' parameter is set to 1. Type should be `LATENT`.
        - `latent2`: The second latent input option. This input is selected if the 'Input' parameter is set to 2. Type should be `LATENT`.
    - Outputs:
        - `LATENT`: The selected latent input based on the 'Input' parameter. Type should be `LATENT`.
        - `show_help`: A URL providing additional information and guidance on using the CR_LatentInputSwitch node. Type should be `STRING`.