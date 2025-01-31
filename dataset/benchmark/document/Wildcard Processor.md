- `Wildcard Processor`: The Wildcard Processor node is designed to enhance text inputs by dynamically substituting placeholders with specified or random values. It leverages wildcard and random syntax processing to generate varied outputs based on the given seed, making it ideal for applications requiring text variation and customization.
    - Inputs:
        - `prompt` (Required): The primary text input containing placeholders for dynamic substitution. It serves as the base for wildcard and random syntax processing, directly influencing the generated output. Type should be `STRING`.
        - `seed` (Required): A numerical value used to initialize the random number generator, ensuring the reproducibility of text variations. It plays a crucial role in the deterministic transformation of the input text. Type should be `INT`.
    - Outputs:
        - `string`: The processed text with wildcards and optional elements dynamically replaced, ready for further use or display. Type should be `STRING`.
