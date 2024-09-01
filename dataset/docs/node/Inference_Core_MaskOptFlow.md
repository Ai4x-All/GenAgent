- `Inference_Core_MaskOptFlow`: The node 'Inference_Core_MaskOptFlow' is designed to process optical flow data by applying a mask to it, effectively filtering the optical flow based on the provided mask. This preprocessing step is crucial for tasks that require focused analysis on specific regions of the optical flow, enhancing the accuracy and relevance of the flow data for subsequent processing stages.
    - Parameters:
    - Inputs:
        - `optical_flow`: The 'optical_flow' parameter represents the optical flow data to be processed. It is essential for determining the motion between two images or frames. Type should be `OPTICAL_FLOW`.
        - `mask`: The 'mask' parameter is used to specify the regions of interest within the optical flow data. It plays a critical role in filtering and refining the flow data for targeted analysis. Type should be `MASK`.
    - Outputs:
        - `OPTICAL_FLOW`: The modified optical flow data, filtered through the applied mask, ready for further analysis or processing. Type should be `OPTICAL_FLOW`.
        - `PREVIEW_IMAGE`: A visual representation of the masked optical flow, providing a preview of the effect of the mask on the flow data. Type should be `IMAGE`.