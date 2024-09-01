- `DetailerForEachDebugPipe`: The node 'DetailerForEachDebugPipe' is designed to facilitate debugging within the context of detailer pipes, providing insights and diagnostics that help in understanding and improving the flow of data and operations. It aims to enhance the development and troubleshooting process by offering a detailed view into the workings of detailer pipes.
    - Parameters:
        - `guide_size`: unknown Type should be `FLOAT`.
        - `guide_size_for`: unknown Type should be `BOOLEAN`.
        - `max_size`: unknown Type should be `FLOAT`.
        - `seed`: unknown Type should be `INT`.
        - `steps`: unknown Type should be `INT`.
        - `cfg`: unknown Type should be `FLOAT`.
        - `sampler_name`: unknown Type should be `COMBO[STRING]`.
        - `scheduler`: unknown Type should be `COMBO[STRING]`.
        - `denoise`: unknown Type should be `FLOAT`.
        - `feather`: unknown Type should be `INT`.
        - `noise_mask`: unknown Type should be `BOOLEAN`.
        - `force_inpaint`: unknown Type should be `BOOLEAN`.
        - `wildcard`: A string input that allows for dynamic prompts or additional debugging information to be passed into the pipe, enhancing the flexibility and depth of debugging. Type should be `STRING`.
        - `refiner_ratio`: unknown Type should be `FLOAT`.
        - `cycle`: unknown Type should be `INT`.
        - `inpaint_model`: unknown Type should be `BOOLEAN`.
        - `noise_mask_feather`: unknown Type should be `INT`.
    - Inputs:
        - `image`: unknown Type should be `IMAGE`.
        - `segs`: unknown Type should be `SEGS`.
        - `basic_pipe`: unknown Type should be `BASIC_PIPE`.
        - `detailer_hook`: unknown Type should be `DETAILER_HOOK`.
        - `refiner_basic_pipe_opt`: unknown Type should be `BASIC_PIPE`.
    - Outputs:
        - `image`: unknown Type should be `IMAGE`.
        - `segs`: unknown Type should be `SEGS`.
        - `basic_pipe`: unknown Type should be `BASIC_PIPE`.
        - `cropped`: unknown Type should be `IMAGE`.
        - `cropped_refined`: unknown Type should be `IMAGE`.
        - `cropped_refined_alpha`: unknown Type should be `IMAGE`.
        - `cnet_images`: unknown Type should be `IMAGE`.