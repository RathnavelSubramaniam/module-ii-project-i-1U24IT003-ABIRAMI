# AI-Powered Medical Assistant

## Overview

The **AI-Powered Medical Assistant** is a healthcare information system developed using **Large Language Models (LLMs)** and **Retrieval-Augmented Generation (RAG)**. It provides medical information through a local LLaMA 2 13B model and improves responses by retrieving relevant information from a medical diagnosis manual.

## Technologies

* Python
* LLaMA 2 13B
* LangChain
* ChromaDB
* Hugging Face
* Sentence Transformers
* PyMuPDF

## Workflow

```text
User Question
     ↓
Medical Knowledge Retrieval
     ↓
Relevant Context
     ↓
LLaMA 2 13B
     ↓
Medical Response
```

## Key Features

* Medical question answering
* Prompt-based LLM responses
* Medical document retrieval
* Semantic search using embeddings
* Context-based response generation
* Groundedness and relevance evaluation

## RAG Details

The medical diagnosis manual is divided into chunks and converted into embeddings using **all-MiniLM-L6-v2**. The embeddings are stored in **ChromaDB**, and the top 5 relevant chunks are retrieved for each query.

## Evaluation

The system evaluates responses based on **groundedness** and **relevance**, helping measure how accurately responses are supported by the retrieved medical context.

## Limitations

* Responses may still contain errors.
* Retrieval quality affects response quality.
* Medical information may require regular updates.
* The system should not replace professional medical diagnosis.

## Future Scope

* Add more trusted medical sources.
* Improve retrieval and reranking.
* Add citations.
* Develop a web/Streamlit interface.
* Improve medical safety and evaluation.

## Conclusion

The project demonstrates how **LLMs and RAG can be combined to build a context-aware medical assistant**. RAG provides relevant medical knowledge to the LLM, improving the reliability and grounding of generated responses.
