- `LLMSemanticSplitterNodeParser`: This node is designed to parse documents semantically using a specified language model for embeddings, optionally incorporating sentence splitting, metadata inclusion, and relationship analysis between sequential elements. It aims to enhance the understanding and structuring of text by leveraging deep learning models to identify and organize semantic components.
    - Inputs:
        - `document` (Required): The primary text document to be parsed. It serves as the core input for semantic analysis and structuring. Type should be `DOCUMENT`.
        - `llm_embed_model` (Required): The language model used for generating embeddings, which is crucial for the semantic parsing process. Type should be `LLM_EMBED_MODEL`.
        - `buffer_size` (Optional): Determines the size of the processing buffer, affecting the granularity of parsing and potentially the performance. Type should be `INT`.
        - `sentence_splitter` (Optional): An optional model or method for splitting the document into sentences, enhancing the semantic parsing accuracy. Type should be `LLM_SENTENCE_SPLITTER`.
        - `include_metadata` (Optional): Flag to include metadata in the parsing process, enriching the semantic understanding of the document. Type should be `BOOLEAN`.
        - `include_prev_next_rel` (Optional): Flag to analyze and include the relationships between sequential elements, offering deeper insights into the document structure. Type should be `BOOLEAN`.
    - Outputs:
        - `llm_node_parser`: The result of the semantic parsing process, structured to reflect the semantic components and relationships identified within the document. Type should be `LLM_NODE_PARSER`.