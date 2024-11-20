- `AV_OpenAIApi`: The AV_OpenAIApi node facilitates the creation of an API client for interacting with OpenAI's services, enabling the integration of OpenAI's language model capabilities within the ArtVenture ecosystem. It abstracts the authentication and setup process, making it easier to leverage OpenAI's API for various language processing tasks.
    - Inputs:
        - `openai_api_key` (Required): The API key for authenticating requests to OpenAI's services. It is essential for enabling secure communication with OpenAI's API. Type should be `STRING`.
        - `endpoint` (Required): The URL endpoint for OpenAI's API. It defaults to OpenAI's official API endpoint but can be customized if needed. Type should be `STRING`.
    - Outputs:
        - `llm_api`: Returns an instance of the OpenAIApi, configured and ready to interact with OpenAI's language models. Type should be `LLM_API`.