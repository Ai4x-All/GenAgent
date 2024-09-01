- `ConversableAgentCreatorAdvanced`: This node specializes in creating advanced conversable agents with customizable capabilities, including the integration of large language models (LLMs) and personalized system messages. It allows for the creation of AI agents that can handle complex interactions and provide tailored responses based on specific configurations.
    - Parameters:
        - `name`: The name parameter specifies the identity of the conversable agent being created, serving as a unique identifier and a label for interaction. Type should be `STRING`.
        - `system_message`: The system_message parameter defines the initial message or instruction set that the agent uses to guide its interactions, setting the tone and context for its operation. Type should be `STRING`.
        - `default_auto_reply`: Specifies a default response for the agent to use when it cannot generate a specific reply, ensuring a fallback communication. Type should be `STRING`.
        - `description`: A brief description of the agent's purpose or capabilities, used for identification or reference by other agents. Type should be `STRING`.
    - Inputs:
        - `llm_model`: The llm_model parameter allows for the specification of a large language model to empower the agent with advanced understanding and response generation capabilities. Type should be `LLM_MODEL`.
    - Outputs:
        - `agent`: The output is a conversable agent configured with the provided parameters, ready for interaction and capable of complex task handling. Type should be `AGENT`.