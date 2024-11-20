- `LayerStyle_ ColorOverlay V2`: The ColorOverlay V2 node applies a color overlay to an image, allowing for the adjustment of blend mode, opacity, and color to achieve various visual effects. It supports the inversion of a mask for more complex layering and styling options.
    - Inputs:
        - `background_image` (Required): Specifies the background image over which the color overlay will be applied. It is a foundational element for the overlay effect. Type should be `IMAGE`.
        - `layer_image` (Required): Defines the layer image to which the color overlay effect will be applied, enabling the creation of layered visual effects. Type should be `IMAGE`.
        - `invert_mask` (Required): Determines whether the mask applied to the layer image should be inverted, offering additional control over the overlay effect. Type should be `BOOLEAN`.
        - `blend_mode` (Required): Specifies the blending mode used for combining the color overlay with the layer image, affecting the overall visual outcome. The correct data type should reflect a custom enumeration or selection type, not a standard Python data type. Type should be `COMBO[STRING]`.
        - `opacity` (Required): Controls the opacity level of the color overlay, allowing for fine-tuning of the effect's intensity. Type should be `INT`.
        - `color` (Required): Sets the color of the overlay, enabling customization of the visual effect. Type should be `STRING`.
        - `layer_mask` (Optional): Optional mask that can be applied to the layer image for more precise control over the overlay effect. Type should be `MASK`.
    - Outputs:
        - `image`: The resulting image after applying the color overlay effect, incorporating adjustments made through the node's parameters. Type should be `IMAGE`.