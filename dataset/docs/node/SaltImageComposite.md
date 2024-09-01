- `SaltImageComposite`: The SaltImageComposite node is designed for creating complex image compositions by blending or layering multiple images according to specified schedules. This node enables the dynamic combination of images, facilitating the creation of visually rich and varied outputs.
    - Parameters:
        - `mode`: Defines the method of blending the two image sets. The mode determines how images_a and images_b are combined, influencing the visual outcome of the composite. Type should be `COMBO[STRING]`.
    - Inputs:
        - `images_a`: The first set of images to be used in the compositing process. These images serve as one of the primary layers for the composition. Type should be `IMAGE`.
        - `images_b`: The second set of images to be used in the compositing process. These images act as the other primary layer for the composition, which will be blended with the first set based on the specified mode. Type should be `IMAGE`.
        - `masks`: Optional masks that can be applied to the images during the compositing process. Masks allow for more controlled blending by specifying areas of the images to be affected or protected. Type should be `MASK`.
        - `blend_schedule`: An optional schedule that dictates the blending intensity or method over time, allowing for dynamic changes in the compositing process. Type should be `LIST`.
    - Outputs:
        - `images`: The resulting images after applying the compositing operations. This output showcases the final composites, blending all input images according to the defined modes and schedules. Type should be `IMAGE`.