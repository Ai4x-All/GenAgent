- `Camera_AnglesStylerAdvanced`: The Camera_AnglesStylerAdvanced node is designed to manipulate and enhance images by adjusting their camera angles, leveraging 3D geometry and perspective transformations. This node applies complex algorithms to simulate changes in elevation and azimuth of the camera's viewpoint, aiming to achieve a more dynamic or aesthetically pleasing composition.
    - Inputs:
        - `text_positive_g` (Required): Specifies the positive aspects to emphasize in the generated text, guiding the generation towards favorable outcomes. Type should be `STRING`.
        - `text_positive_l` (Required): Defines the local positive attributes to be highlighted in the text, focusing on specific details or elements. Type should be `STRING`.
        - `text_negative` (Required): Indicates the negative aspects to be minimized or avoided in the text generation, aiming to steer clear of undesirable outcomes. Type should be `STRING`.
        - `camera_angles` (Required): Controls the simulation of camera angles, including elevation and azimuth, to adjust the perspective in the generated images. Type should be `COMBO[STRING]`.
        - `negative_prompt_to` (Required): Targets specific negative prompts for transformation, aiming to convert them into a more positive or neutral context. Type should be `COMBO[STRING]`.
        - `log_prompt` (Required): Logs the prompts used for generating text, aiding in the tracking and refinement of the generation process. Type should be `BOOLEAN`.
    - Outputs:
        - `text_positive_g`: Generates globally positive text, reflecting the overall positive outcome of the transformation. Type should be `STRING`.
        - `text_positive_l`: Produces locally positive text, highlighting specific positive details or elements. Type should be `STRING`.
        - `text_positive`: Outputs text that has been positively influenced by the specified prompts and camera angle adjustments. Type should be `STRING`.
        - `text_negative_g`: Generates globally negative text, which may serve as a contrast or control to the positive outputs. Type should be `STRING`.
        - `text_negative_l`: Produces locally negative text, focusing on specific negative details or elements for contrast or control purposes. Type should be `STRING`.
        - `text_negative`: Outputs text that remains negatively influenced, serving as a baseline or control for comparison. Type should be `STRING`.
