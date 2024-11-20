- `SplitSigmasDenoise`: The SplitSigmasDenoise node is designed to partition a given sequence of sigmas into two distinct sequences based on a denoising factor. This operation facilitates the customization of the sampling process by allowing for the adjustment of the sequence length according to the desired level of denoising, thereby enabling more precise control over the generation quality.
    - Inputs:
        - `sigmas` (Required): The sequence of sigmas to be split. It represents the noise levels at different steps of the generation process, playing a crucial role in determining the granularity of the split and the subsequent denoising effect. Type should be `SIGMAS`.
        - `denoise` (Required): A factor determining the extent of denoising by adjusting the split point in the sigma sequence. It directly influences the balance between the high and low sigma sequences, thereby affecting the overall denoising strategy. Type should be `FLOAT`.
    - Outputs:
        - `high_sigmas`: The portion of the sigma sequence with higher values, representing the initial, less denoised stages of the generation process. Type should be `SIGMAS`.
        - `low_sigmas`: The portion of the sigma sequence with lower values, indicating the later, more denoised stages of the generation process. Type should be `SIGMAS`.