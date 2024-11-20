- `LayerStyle_ Stroke V2`: The Stroke V2 node is designed to apply advanced stroke effects to images within a layer-based design system. It enhances visual aesthetics by allowing for detailed customization of stroke properties such as color, width, and blending modes.
    - Inputs:
        - `background_image` (Required): The background image over which the stroke effect will be applied. It serves as the canvas for the stroke enhancements. Type should be `IMAGE`.
        - `layer_image` (Required): The layer image to which the stroke effect will be directly applied. This image is modified based on the stroke settings. Type should be `IMAGE`.
        - `invert_mask` (Required): A boolean parameter that determines whether the mask applied to the layer image should be inverted, affecting the area where the stroke is applied. Type should be `BOOLEAN`.
        - `blend_mode` (Required): Specifies the blending mode used to combine the stroke effect with the layer image, influencing the final visual outcome. Type should be `COMBO[STRING]`.
        - `opacity` (Required): Controls the opacity level of the stroke effect, allowing for fine-tuning of its visibility on the layer image. Type should be `INT`.
        - `stroke_grow` (Required): Determines the growth or shrinkage of the stroke effect relative to the original layer boundaries, enabling more precise control over the effect's spread. Type should be `INT`.
        - `stroke_width` (Required): Sets the width of the stroke effect, defining the thickness of the applied stroke around the layer image. Type should be `INT`.
        - `blur` (Required): Adjusts the blur intensity of the stroke effect, offering the ability to soften or sharpen the edges of the stroke. Type should be `INT`.
        - `stroke_color` (Required): Defines the color of the stroke effect, allowing for customization to match the design's color scheme. Type should be `STRING`.
        - `layer_mask` (Optional): An optional mask that can be applied to the layer image, defining specific areas where the stroke effect should or should not be applied. Type should be `MASK`.
    - Outputs:
        - `image`: The resulting image after applying the stroke V2 effect, showcasing the enhanced visual layer with the specified stroke properties. Type should be `IMAGE`.