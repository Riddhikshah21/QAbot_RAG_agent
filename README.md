# QAbot_RAG_agent

RAG application has 2 components:
    1. Indexing 
        a. Load - load data 
        b. Split - split large document into smaller chunks 
        c. Store - store embedding of the data into a vector database

    2. Retrieval and generation  
        a. Retrieve - retrieve relevant data from vector database based on the similarity search on the indexing and pass the retrieved data as context to the model.
        b. Generate - prompt containing the context and query to the LLM for generating response. 
        
 Components from Langchain suite of integrations:
    1. Chat model 
    2. Embedding model
    3. Vector store
 
 LangGraph:
    - Orchestration framework to implement retrieval and generation steps. 
    - Library to build stateful, multi-actor applications with LLMs, used to create agent and multi-agent workflows
 
 LangSmith:
    - Used to understand the implementation steps of LLM with multiple invocation of LLM calls. 
    - Inspect each chain and agent implemented using LangSmith
 