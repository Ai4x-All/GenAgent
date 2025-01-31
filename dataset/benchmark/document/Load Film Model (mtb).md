- `Load Film Model (mtb)`: The MTB_LoadFilmModel node is designed to load FILM models for frame interpolation tasks, supporting a variety of model formats and ensuring the model is correctly loaded for further processing.
    - Inputs:
        - `film_model` (Required): Specifies the FILM model to be loaded, affecting which specific model file is accessed and utilized in frame interpolation tasks. Type should be `COMBO[STRING]`.
    - Outputs:
        - `film_model`: Returns an instance of the loaded FILM model, ready for frame interpolation operations. Type should be `FILM_MODEL`.
