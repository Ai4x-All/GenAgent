- `FaceEmbedDistance`: The FaceEmbedDistance node calculates the distance between facial embeddings using cosine or Euclidean (L2) metrics. It supports normalization of embeddings for distance calculation, enabling a versatile approach to measuring facial similarity or dissimilarity.
    - Inputs:
        - `analysis_models` (Required): Specifies the face analysis models to be used for generating embeddings from the input images. It plays a critical role in the accuracy of the distance measurements. Type should be `ANALYSIS_MODELS`.
        - `reference` (Required): The reference image against which other images are compared. This image is used to generate a facial embedding for similarity comparison. Type should be `IMAGE`.
        - `image` (Required): The image to be compared against the reference. It is used to generate a facial embedding for calculating the distance to the reference embedding. Type should be `IMAGE`.
        - `similarity_metric` (Required): Defines the metric used for calculating the distance between embeddings. Options include 'L2_norm', 'cosine', and 'euclidean', affecting the comparison's sensitivity and outcome. Type should be `COMBO[STRING]`.
        - `filter_thresh` (Required): A threshold for filtering out distances above a certain value, enhancing the focus on closer matches. Type should be `FLOAT`.
        - `filter_best` (Required): Limits the number of results to the best matches below the specified threshold, optimizing the search for similarity. Type should be `INT`.
        - `generate_image_overlay` (Required): A boolean indicating whether to overlay the reference image on top of the comparison image, visually representing the similarity measurement. Type should be `BOOLEAN`.
    - Outputs:
        - `IMAGE`: The image result of overlaying the reference image on the comparison image, if enabled, providing a visual representation of the similarity. Type should be `IMAGE`.
        - `distance`: The calculated distance between the facial embeddings of the reference and comparison images, quantifying their similarity. Type should be `FLOAT`.
