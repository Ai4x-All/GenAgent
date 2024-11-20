- `ImpactIPAdapterApplySEGS`: This node applies an IP Adapter to SEGS (segmentation elements), enhancing or modifying them based on a set of parameters and a reference image. It allows for the dynamic adjustment of segmentation elements through image processing techniques and neural network models, facilitating complex image manipulation tasks.
    - Inputs:
        - `segs` (Required): The segmentation elements to be processed, typically including information such as crop regions and masks. Type should be `SEGS`.
        - `ipadapter_pipe` (Required): A pipeline of models or functions that the IP Adapter will use to process the segmentation elements. Type should be `IPADAPTER_PIPE`.
        - `weight` (Required): A parameter controlling the influence of the IP Adapter on the segmentation elements. Type should be `FLOAT`.
        - `noise` (Required): An optional noise parameter that can be applied for variability in the adaptation process. Type should be `FLOAT`.
        - `weight_type` (Required): Specifies the type of weighting mechanism used in the adaptation process. Type should be `COMBO[STRING]`.
        - `start_at` (Required): Defines the starting point within the pipeline for applying the IP Adapter. Type should be `FLOAT`.
        - `end_at` (Required): Specifies the endpoint within the pipeline for the application of the IP Adapter. Type should be `FLOAT`.
        - `unfold_batch` (Required): Determines whether the processing should unfold in batches for efficiency. Type should be `BOOLEAN`.
        - `faceid_v2` (Required): An optional parameter for face identification, relevant in certain contexts. Type should be `BOOLEAN`.
        - `weight_v2` (Required): A secondary weight parameter, potentially used for more nuanced control. Type should be `FLOAT`.
        - `context_crop_factor` (Required): Adjusts the crop region in relation to the context, affecting how much of the surrounding area is considered in the adaptation. Type should be `FLOAT`.
        - `reference_image` (Required): The reference image against which the segmentation elements are adapted or modified. Type should be `IMAGE`.
        - `combine_embeds` (Optional): Determines how embeddings are combined in the adaptation process, with options such as 'concat'. Type should be `COMBO[STRING]`.
        - `neg_image` (Optional): An optional negative image that can be used for contrast or as a counter-reference in the adaptation. Type should be `IMAGE`.
    - Outputs:
        - `segs`: The enhanced or modified segmentation elements after applying the IP Adapter. Type should be `SEGS`.