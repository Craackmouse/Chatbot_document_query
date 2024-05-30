
## Opensource LLM based RAG for information retrieval from 100 research papers

# Overview of approach:

    Different opensource light weight LLMs for each task. Embedding creation, Summerization of retrieved chunks and Q&A
    Fassai for indexing (IndexIVFFlat trained)
    Ngrok for serving flask through colab

# Discussion on improvement (Approach not taken due to unavailability of free gpu credits):

    Text extraction using LLM to retain table and chart info better

    Finetuning on Research papers

    More advanced LLM can also be utilized which can handle all the three task together.

    Prompting can be leveraged to further improve the output.

    Memory chain, aggregation of reasoning, pdf level llm agents are few other techniques that can be leveraged to improve the performance and experience.

# How to test code:

    open colab in your account.
    upload extracted pdf file directory and update path.
    change runtime type and set T4 GPU.
    execute all cell then at end you will get ngrok tunnel like "https://*********.ngrok-free.app".
    open it and use chat.

NOTE: Retrieval code is retrieving relevant chunks from documents. Q&A needs some work for consistant result generation.
