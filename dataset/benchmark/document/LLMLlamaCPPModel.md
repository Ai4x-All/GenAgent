- `LLMLlamaCPPModel`: The LLMLlamaCPPModel node is designed to load and initialize LlamaCPP models, incorporating an embedding model alongside. It facilitates the integration of LlamaCPP models into larger workflows by providing a streamlined mechanism for model loading, including setting up necessary configurations and embedding models for enhanced functionality.
    - Inputs:
        - `model_name` (Required): Specifies the name of the LlamaCPP model to be loaded. This parameter is crucial for identifying the correct model file and initializing the LlamaCPP model accordingly. Type should be `COMBO[STRING]`.
    - Outputs:
        - `model`: Returns a dictionary containing the loaded LlamaCPP model, its name, the associated embedding model, and the embedding model's name. This output is essential for subsequent processing or analysis steps in the workflow. Type should be `LLM_MODEL`.