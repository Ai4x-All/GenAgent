- `ImagesFromBatchSchedule`: This node is designed to generate a batch of images based on a predefined schedule. It leverages a batch value schedule list to select and export images from an input image batch, effectively creating a sequence or collection of images according to specified scheduling criteria. The functionality is inspired by and extends the capabilities of the ComfyUI-Image-Selector, facilitating advanced image batch processing and manipulation.
    - Parameters:
        - `text`: The scheduling criteria or instructions provided as text, which dictate how images are selected and organized from the batch. Type should be `STRING`.
        - `current_frame`: Specifies the current frame in the scheduling sequence, used to determine which images are selected. Type should be `INT`.
        - `max_frames`: The maximum number of frames to consider in the scheduling process, defining the upper limit of the batch processing. Type should be `INT`.
        - `print_output`: A boolean flag indicating whether to print the scheduling process's output for debugging or informational purposes. Type should be `BOOLEAN`.
    - Inputs:
        - `images`: The input image batch from which images are to be selected and processed according to the batch schedule. This parameter is crucial for defining the source images for the scheduling operation. Type should be `IMAGE`.
    - Outputs:
        - `image`: The output is a single image or a batch of images that have been selected and processed according to the input batch schedule. This collection of images is ready for further use or analysis. Type should be `IMAGE`.