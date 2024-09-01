- `VRAM_Debug`: The VRAM_Debug node is designed to monitor and manage video RAM (VRAM) usage within a computational environment. It provides functionalities to clear memory caches, unload all models from memory, and perform garbage collection to free up VRAM. This node is particularly useful for optimizing memory usage and preventing out-of-memory errors during intensive computational tasks.
    - Parameters:
        - `empty_cache`: Specifies whether to clear PyTorch's cache, potentially freeing up a significant amount of VRAM. Type should be `BOOLEAN`.
        - `gc_collect`: Determines whether garbage collection is performed, helping to free up unused memory and optimize VRAM usage. Type should be `BOOLEAN`.
        - `unload_all_models`: Indicates whether all models should be unloaded from memory, which can drastically reduce VRAM usage. Type should be `BOOLEAN`.
    - Inputs:
        - `any_input`: Allows for any additional input to be passed through the node, offering flexibility in its application. Type should be `*`.
        - `image_pass`: An optional image data that can be passed through the node without modification. Type should be `IMAGE`.
        - `model_pass`: An optional model data that can be passed through the node without modification. Type should be `MODEL`.
    - Outputs:
        - `any_output`: Returns any additional input passed to the node, allowing for flexible data flow. Type should be `*`.
        - `image_pass`: Returns the optional image data passed through the node without modification. Type should be `IMAGE`.
        - `model_pass`: Returns the optional model data passed through the node without modification. Type should be `MODEL`.
        - `freemem_before`: Provides the amount of free VRAM before the node's operations were executed. Type should be `INT`.
        - `freemem_after`: Provides the amount of free VRAM after the node's operations, highlighting the effectiveness of memory management. Type should be `INT`.