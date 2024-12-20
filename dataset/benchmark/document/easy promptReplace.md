- `easy promptReplace`: The `promptReplace` node is designed to dynamically modify text prompts based on a set of replacement rules. It allows for the customization of text by replacing specified phrases or words with alternatives, supporting a straightforward approach to text manipulation. This functionality is particularly useful for generating or altering text prompts in a flexible manner, accommodating a wide range of text manipulation needs.
    - Inputs:
        - `prompt` (Required): The initial text prompt that will be modified based on the find and replace parameters provided. Type should be `STRING`.
        - `find1` (Optional): The first phrase or word to search for in the prompt for replacement. Type should be `STRING`.
        - `replace1` (Optional): The replacement text for the first search term found by `find1`. Type should be `STRING`.
        - `find2` (Optional): The second phrase or word to search for in the prompt for replacement. Type should be `STRING`.
        - `replace2` (Optional): The replacement text for the second search term found by `find2`. Type should be `STRING`.
        - `find3` (Optional): The third phrase or word to search for in the prompt for replacement. Type should be `STRING`.
        - `replace3` (Optional): The replacement text for the third search term found by `find3`. Type should be `STRING`.
    - Outputs:
        - `prompt`: The output is a modified version of the input text, with specified phrases or words replaced according to the defined rules. Type should be `STRING`.
