## LangChain PDF Chatbot
This project implements a chatbot based on Large Language Models (LLMs) using the LangChain framework, capable of answering questions related to the content of a PDF file. This chatbot works by utilizing HuggingFace Embeddings and FAISS for information retrieval, as well as the google/flan-t5-base model from HuggingFace Transformers for response generation.

## Features
- PDF Document Loading: Ability to load and process PDF files using PyPDFLoader.
- Text Splitting: Dividing documents into smaller chunks with RecursiveCharacterTextSplitter for optimal processing.
- Embedding and Vector Store: Using the sentence-transformers/all-MiniLM-L6-v2 model to generate embeddings and store them in the FAISS vector database.
- Large Language Model: Utilizing the google/flan-t5-base model from HuggingFace Transformers to generate relevant answers to questions.
- Conversational Memory: Maintaining conversation history with ConversationBufferMemory to provide contextual and relevant responses.
- Information Retrieval: Efficiently retrieving relevant information from PDF documents to answer user questions using ConversationalRetrievalChain.


## What I've Learned from This Project
For a newcomer to the LLM field, completing this project taught me the following key experiences:

- Familiarity with LangChain: The most significant achievement was understanding and working with the LangChain framework. I learned how to connect various components (such as Document Loaders, Text Splitters, Embeddings, Vector Stores, LLMs, Chains, and Memory) to build a complete system.
- Concept of RAG (Retrieval-Augmented Generation): This project served as a practical example of RAG. I understood how retrieving relevant information from a knowledge base (here, a PDF) can lead to more accurate and fact-based answers from an LLM, rather than solely relying on the model's pre-trained knowledge.
- Document Processing: By using PyPDFLoader and RecursiveCharacterTextSplitter, I learned how to load large documents and divide them into manageable chunks for LLM processing.
- Embeddings and Vector Databases (Vector Stores): I grasped how embeddings convert text into numerical vectors and why these vectors are crucial for semantic search. I also learned how to use FAISS as a vector database for efficient storage and retrieval of these embeddings.
- HuggingFace Models: I became familiar with using various HuggingFace models (such as sentence-transformers/all-MiniLM-L6-v2 for Embeddings and google/flan-t5-base as the LLM) within LangChain.
- Chatbot Memory Management (Conversation Memory): I understood the importance of preserving conversation history to create a continuous and contextual chatbot experience using ConversationBufferMemory.
- LLM Project Structuring: This project provided me with an overall view of the steps involved in building an LLM-based application, from data loading to response generation.
