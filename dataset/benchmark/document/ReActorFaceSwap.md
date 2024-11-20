- `ReActorFaceSwap`: The ReActorFaceSwap node specializes in performing fast face swaps within images, leveraging advanced algorithms to seamlessly replace faces in a given image with those from another source. This node is designed to handle the complexities of face swapping, including alignment, scaling, and blending, to produce natural-looking results.
    - Inputs:
        - `enabled` (Required): Indicates if the face swap operation is currently enabled, controlling whether the swapping process should proceed. Type should be `BOOLEAN`.
        - `input_image` (Required): The image that serves as either the source or target for the face swap operation, depending on the context of the swap. Type should be `IMAGE`.
        - `swap_model` (Required): Specifies the model used for the face swapping process, determining the algorithm and parameters for the swap. Type should be `COMBO[STRING]`.
        - `facedetection` (Required): unknown Type should be `COMBO[STRING]`.
        - `face_restore_model` (Required): unknown Type should be `COMBO[STRING]`.
        - `face_restore_visibility` (Required): unknown Type should be `FLOAT`.
        - `codeformer_weight` (Required): unknown Type should be `FLOAT`.
        - `detect_gender_input` (Required): unknown Type should be `COMBO[STRING]`.
        - `detect_gender_source` (Required): unknown Type should be `COMBO[STRING]`.
        - `input_faces_index` (Required): unknown Type should be `STRING`.
        - `source_faces_index` (Required): unknown Type should be `STRING`.
        - `console_log_level` (Required): unknown Type should be `COMBO[INT]`.
        - `source_image` (Optional): unknown Type should be `IMAGE`.
        - `face_model` (Optional): unknown Type should be `FACE_MODEL`.
        - `face_boost` (Optional): unknown Type should be `FACE_BOOST`.
    - Outputs:
        - `image`: The final image after the face swap operation has been completed, showcasing the seamless integration of the swapped face. Type should be `IMAGE`.
        - `face_model`: The model used for the face swap, providing details about the algorithm and parameters applied. Type should be `FACE_MODEL`.