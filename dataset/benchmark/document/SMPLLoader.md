- `SMPLLoader`: The SMPLLoader node is designed to load and process SMPL model data from specified files, facilitating the integration of SMPL models into motion analysis and synthesis workflows.
    - Inputs:
        - `smpl` (Required): Specifies the file name of the SMPL model to be loaded. This file contains essential data for motion synthesis, including pose parameters. Type should be `COMBO[STRING]`.
        - `smpl_model` (Required): Determines the specific SMPL model to be used, affecting the interpretation of the loaded SMPL data. Type should be `COMBO[STRING]`.
    - Outputs:
        - `smpl`: Outputs a tuple containing the path to the SMPL model, pose parameters (thetas), and metadata, ready for further processing or visualization. Type should be `SMPL`.