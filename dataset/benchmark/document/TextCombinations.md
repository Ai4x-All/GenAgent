- `TextCombinations`: The TextCombinations node is designed to generate a variety of text combinations based on predefined text inputs and operations. It allows for the dynamic mixing and matching of text elements to create new, composite strings according to specified operations, making it a versatile tool for text manipulation and generation.
    - Inputs:
        - `text1` (Required): The first text input that can be dynamically combined with other text inputs according to the specified operation. Type should be `STRING`.
        - `text2` (Required): The second text input that can be combined with the first text input and potentially others, depending on the operation defined. Type should be `STRING`.
        - `operation` (Required): Defines the specific combination operation to be applied to the text inputs, determining how they are mixed and matched to generate the output. Type should be `COMBO[STRING]`.
        - `delimiter` (Required): A string used to separate text elements in the output, allowing for customization of the output format. Type should be `STRING`.
        - `use_seed` (Required): A boolean flag indicating whether a seed should be used to generate deterministic combinations. Type should be `COMBO[STRING]`.
        - `seed` (Required): An integer seed value used to ensure deterministic output when combining text inputs, if 'use_seed' is true. Type should be `INT`.
    - Outputs:
        - `output1`: The first resulting string after applying the specified combination operation to the input texts. Type should be `STRING`.
        - `output2`: The second resulting string after applying the specified combination operation to the input texts. Type should be `STRING`.