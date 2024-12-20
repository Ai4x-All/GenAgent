- `EditDetailerPipeSDXL`: The EditDetailerPipeSDXL node is designed to enhance and refine the details of inputs through a sophisticated editing pipeline. It allows for the integration of various models and techniques, including LoRA and Wildcards, to achieve more precise and impactful modifications.
    - Inputs:
        - `detailer_pipe` (Required): Represents the initial detailer pipeline to be enhanced or modified. It serves as the foundation for further refinements. Type should be `DETAILER_PIPE`.
        - `wildcard` (Required): Allows for dynamic text input that can be used to modify or influence the detailer pipeline in a flexible manner. Type should be `STRING`.
        - `Select to add LoRA` (Required): Provides a selection mechanism for integrating LoRA (Low-Rank Adaptation) techniques into the text, enhancing its detail and specificity. Type should be `COMBO[STRING]`.
        - `Select to add Wildcard` (Required): Enables the selection of predefined Wildcards to be added to the text, offering additional customization and detail enhancement. Type should be `COMBO[STRING]`.
        - `model` (Optional): Specifies the model to be used in the detailer pipeline, contributing to the enhancement process. Type should be `MODEL`.
        - `clip` (Optional): Defines the CLIP model to be integrated into the pipeline for improved content understanding and manipulation. Type should be `CLIP`.
        - `vae` (Optional): Specifies the VAE model to be used for generating or modifying content within the pipeline. Type should be `VAE`.
        - `positive` (Optional): Defines positive conditioning to guide the generation or modification process towards desired attributes. Type should be `CONDITIONING`.
        - `negative` (Optional): Specifies negative conditioning to steer the generation or modification process away from undesired attributes. Type should be `CONDITIONING`.
        - `refiner_model` (Optional): Specifies an additional model for refining the details further in the pipeline. Type should be `MODEL`.
        - `refiner_clip` (Optional): Defines an additional CLIP model for enhanced content understanding and manipulation in the refinement process. Type should be `CLIP`.
        - `refiner_positive` (Optional): Defines additional positive conditioning for the refinement process, enhancing desired attributes. Type should be `CONDITIONING`.
        - `refiner_negative` (Optional): Specifies additional negative conditioning for the refinement process, avoiding undesired attributes. Type should be `CONDITIONING`.
        - `bbox_detector` (Optional): Specifies a bounding box detector to be used for object detection and localization within the pipeline. Type should be `BBOX_DETECTOR`.
        - `sam_model` (Optional): Specifies a SAM model to be integrated for semantic adjustment or manipulation within the pipeline. Type should be `SAM_MODEL`.
        - `segm_detector` (Optional): Defines a segmentation detector to be used for segmenting different parts or objects within the content. Type should be `SEGM_DETECTOR`.
        - `detailer_hook` (Optional): Provides a hook for custom detailer functions or modifications to be applied within the pipeline. Type should be `DETAILER_HOOK`.
    - Outputs:
        - `detailer_pipe`: Outputs the enhanced detailer pipeline, incorporating all specified models, techniques, and modifications. Type should be `DETAILER_PIPE`.
