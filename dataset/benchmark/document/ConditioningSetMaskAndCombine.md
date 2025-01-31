- `ConditioningSetMaskAndCombine`: This node is designed to apply masks to conditioning data, adjusting the conditioning based on specified masks and their strengths. It combines the functionality of setting masks and combining conditioned data, allowing for the dynamic alteration of conditioning areas within a given dataset.
    - Inputs:
        - `positive_i` (Required): Specifies a set of conditioning data to be positively influenced by the corresponding mask, playing a crucial role in tailoring the conditioning to specific areas or aspects of the data. Type should be `CONDITIONING`.
        - `negative_i` (Required): Specifies a set of conditioning data to be negatively influenced by the corresponding mask, essential for excluding or diminishing certain areas or aspects from the conditioning. Type should be `CONDITIONING`.
        - `mask_i` (Required): A mask to be applied to the corresponding conditioning data, determining the areas of influence for positive or negative conditioning adjustments. Type should be `MASK`.
        - `mask_i_strength` (Required): Defines the strength of the mask's influence on the conditioning, allowing for fine-tuned control over how prominently the mask affects the conditioning. Type should be `FLOAT`.
        - `set_cond_area` (Required): Determines whether to set the conditioning area to the bounds of the mask or use the default setting, impacting the scope and precision of conditioning adjustments. Type should be `COMBO[STRING]`.
    - Outputs:
        - `combined_positive`: The combined result of all positive conditioning data after mask application, reflecting the cumulative effect of positive adjustments. Type should be `CONDITIONING`.
        - `combined_negative`: The combined result of all negative conditioning data after mask application, reflecting the cumulative effect of negative adjustments. Type should be `CONDITIONING`.
