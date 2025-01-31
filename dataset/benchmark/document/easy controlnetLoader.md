- `easy controlnetLoader`: The `easy controlnetLoader` node is designed to simplify the process of loading control networks within the ComfyUI framework. It abstracts the complexities involved in fetching and applying control networks to models, offering a streamlined interface for users to easily integrate control networks into their projects.
    - Inputs:
        - `pipe` (Required): Represents the pipeline configuration for which the control network is being loaded. It is essential for ensuring that the control network is applied correctly within the specified pipeline. Type should be `PIPE_LINE`.
        - `image` (Required): The image to which the control network will be applied. This parameter is crucial for visualizing the effects of the control network on specific images. Type should be `IMAGE`.
        - `control_net_name` (Required): Specifies the name of the control network to be loaded. This parameter is crucial as it determines which control network is fetched and applied, directly impacting the behavior of the model. Type should be `COMBO[STRING]`.
        - `control_net` (Optional): An optional parameter that, if provided, specifies a pre-loaded control network to be applied. This allows for more flexibility in using custom or pre-configured control networks. Type should be `CONTROL_NET`.
        - `strength` (Optional): Defines the intensity with which the control network influences the model. This parameter allows users to adjust the impact level of the control network on the output. Type should be `FLOAT`.
        - `scale_soft_weights` (Optional): Adjusts the softness of the weights applied to the control network. This parameter allows for fine-tuning the influence of the control network on the model, enabling users to achieve the desired level of control. Type should be `FLOAT`.
    - Outputs:
        - `pipe`: The updated pipeline configuration, including the applied control network. Type should be `PIPE_LINE`.
        - `positive`: The positive conditioning effects generated by the control network. Type should be `CONDITIONING`.
        - `negative`: The negative conditioning effects generated by the control network. Type should be `CONDITIONING`.
