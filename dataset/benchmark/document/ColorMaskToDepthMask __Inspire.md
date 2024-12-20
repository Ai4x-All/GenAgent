- `ColorMaskToDepthMask __Inspire`: The `ColorMaskToDepthMask` node is designed to convert a color mask into a depth mask based on various specifications including color codes, base values, dilation, and flatten methods. This process involves analyzing the color mask to apply transformations that result in a depth representation, taking into account the specified parameters to adjust the depth effect.
    - Inputs:
        - `color_mask` (Required): `color_mask` is the input tensor representing the color mask to be converted. It plays a crucial role in determining which pixels will be considered for conversion based on the specified mask color. Type should be `IMAGE`.
        - `spec` (Required): `spec` defines the specifications for converting color codes into depth values, including the color code and its corresponding configuration. Type should be `STRING`.
        - `base_value` (Required): `base_value` sets the initial depth value for the mask before applying any color-specific transformations. Type should be `FLOAT`.
        - `dilation` (Required): `dilation` specifies the amount by which to dilate the mask, affecting the depth representation by expanding or contracting the mask areas. Type should be `INT`.
        - `flatten_method` (Required): `flatten_method` determines how multiple mask layers are combined into a single mask, with options such as 'override', 'max', and 'sum'. Type should be `COMBO[STRING]`.
    - Outputs:
        - `mask`: The output is a depth mask tensor, representing the transformed depth mask derived from the original color mask and the specified transformations. Type should be `MASK`.
