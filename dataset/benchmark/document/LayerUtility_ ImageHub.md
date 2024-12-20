- `LayerUtility_ ImageHub`: The ImageHub node serves as a dynamic selector and router for image and mask inputs, allowing for the selection of specific image-mask pairs based on a specified output channel. It facilitates the flexible manipulation and routing of image data within a node network, enabling the creation of complex image processing pipelines.
    - Inputs:
        - `output` (Required): Specifies the output channel to select the corresponding image and mask inputs. It determines which set of inputs (image and mask) will be used for the output. Type should be `INT`.
        - `random_output` (Required): A boolean flag that, if set, could potentially alter the selection logic for choosing the output image and mask, adding an element of randomness to the output selection process. Type should be `BOOLEAN`.
        - `input1_image` (Optional): The first image input option for the node, which can be selected as the output based on the 'output' parameter value. Type should be `IMAGE`.
        - `input1_mask` (Optional): The mask associated with the first image input, providing an option for output selection alongside the corresponding image. Type should be `MASK`.
        - `input2_image` (Optional): The second image input option, selectable based on the output parameter. Type should be `IMAGE`.
        - `input2_mask` (Optional): The mask associated with the second image input, used in conjunction with the corresponding image for output selection. Type should be `MASK`.
        - `input3_image` (Optional): The third image input option, which can be chosen based on the specified output channel. Type should be `IMAGE`.
        - `input3_mask` (Optional): The mask for the third image input, available for selection with its corresponding image based on the output parameter. Type should be `MASK`.
        - `input4_image` (Optional): The fourth image input option, selectable for output based on the specified channel. Type should be `IMAGE`.
        - `input4_mask` (Optional): The mask associated with the fourth image input, selectable alongside the corresponding image. Type should be `MASK`.
        - `input5_image` (Optional): The fifth image input option, which can be selected for output based on the specified channel. Type should be `IMAGE`.
        - `input5_mask` (Optional): The mask for the fifth image input, available for selection with its corresponding image. Type should be `MASK`.
        - `input6_image` (Optional): The sixth image input option, selectable for output based on the output parameter. Type should be `IMAGE`.
        - `input6_mask` (Optional): The mask associated with the sixth image input, used in output selection alongside the corresponding image. Type should be `MASK`.
        - `input7_image` (Optional): The seventh image input option, which can be chosen for output based on the specified channel. Type should be `IMAGE`.
        - `input7_mask` (Optional): The mask for the seventh image input, available for selection with its corresponding image. Type should be `MASK`.
        - `input8_image` (Optional): The eighth image input option, selectable for output based on the output parameter. Type should be `IMAGE`.
        - `input8_mask` (Optional): The mask associated with the eighth image input, used in output selection alongside the corresponding image. Type should be `MASK`.
        - `input9_image` (Optional): The ninth and final image input option, which can be selected for output based on the specified channel. Type should be `IMAGE`.
        - `input9_mask` (Optional): The mask for the ninth image input, available for selection with its corresponding image. Type should be `MASK`.
    - Outputs:
        - `image`: The selected image output based on the specified output channel and input parameters. Type should be `IMAGE`.
        - `mask`: The selected mask output corresponding to the chosen image, based on the specified output channel and input parameters. Type should be `MASK`.
