- `easy applyPowerPaint`: The `easy applyPowerPaint` node is designed to facilitate advanced image manipulation tasks such as text-guided editing, shape-guided creation, object removal, context-aware adjustments, and image outpainting. It leverages a combination of models and techniques, including PowerPaint, to apply complex transformations and enhancements to images based on user-defined parameters.
    - Inputs:
        - `pipe` (Required): Represents the pipeline state, including models and configurations, that the node operates on. It's essential for maintaining the context and progress of image manipulation tasks. Type should be `PIPE_LINE`.
        - `image` (Required): The input image to be manipulated or enhanced. It serves as the primary subject for the node's operations. Type should be `IMAGE`.
        - `mask` (Required): A mask that specifies the areas of the image to be edited or preserved. It plays a crucial role in targeted manipulations such as object removal or area-specific enhancements. Type should be `MASK`.
        - `powerpaint_model` (Required): Specifies the PowerPaint model to be used for the image manipulation task. It determines the underlying algorithm and capabilities available for the operation. Type should be `COMBO[STRING]`.
        - `powerpaint_clip` (Required): Identifies the specific CLIP model associated with PowerPaint, used for understanding and interpreting the content and context of the image. Type should be `COMBO[STRING]`.
        - `dtype` (Required): Defines the data type for the PowerPaint model's computations, affecting performance and precision. Type should be `COMBO[STRING]`.
        - `fitting` (Required): Controls the fitting level of the manipulation to the original image, allowing for fine-tuning the intensity and integration of the applied effects. Type should be `FLOAT`.
        - `function` (Required): Determines the specific manipulation function to be applied, such as text-guided editing or object removal, guiding the node's operation. Type should be `COMBO[STRING]`.
        - `scale` (Required): Adjusts the scale of the manipulation effect, influencing the extent of changes applied to the image. Type should be `FLOAT`.
        - `start_at` (Required): Specifies the starting point for the manipulation process, enabling phased or progressive image editing. Type should be `INT`.
        - `end_at` (Required): Defines the endpoint for the manipulation process, allowing for controlled and precise editing operations. Type should be `INT`.
        - `save_memory` (Required): Optimizes memory usage during the manipulation process, catering to different system capabilities and requirements. Type should be `COMBO[STRING]`.
    - Outputs:
        - `pipe`: The updated pipeline state after applying the PowerPaint manipulations, reflecting the changes and enhancements made to the image. Type should be `PIPE_LINE`.
