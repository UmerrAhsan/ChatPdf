# PDF Chatbot with Langchain and GPT-3.5 Turbo

## Overview

This is the PDF Chatbot project! This chatbot allows users to upload PDFs and engage in conversations about the content using OpenAI GPT-3.5 Turbo. The orchestration is managed through Langchain, leveraging various components like LLM (Language Model), Chains, Prompt Template, Vector Database, and Memory.Just add your open ai key and pdf and you can use this chatbot.

## Components

### 1. Language Model (LLM)

- **Type**: OpenAI GPT-3.5 Turbo
- **Role**: Powers the conversation and responds to user queries.
- **Usage**: Handles natural language understanding and generation.

### 2. Chains

- **Purpose**: Defines the conversation flow and manages context.
- **Role**: Orchestrates the interaction between the user and the chatbot.

### 3. Prompt Template

- **Usage**: Provides a structured format for user interactions.
- **Benefits**: Ensures consistent and effective communication with the language model.

### 4. Vector Database

- **Type**: FAISS
- **Role**: Stores document embeddings for efficient retrieval.
- **Process**: PDFs are chunked into 512 characters with 24 overlaps, and embeddings are created and stored in the vector database.

### 5. Memory

- **Role**: Preserves the context of the ongoing conversation.
- **Functionality**: Helps the chatbot maintain coherence and relevance in responses.

### 6. Embedding Model

- **Type**: OpenAI Text-Embedding-Ada-002
- **Usage**: Generates embeddings for chunks of PDF content.
- **Integration**: Supports the vector database in efficient document representation.

## How to Use

1. **Upload PDF**: Users can upload their PDF documents for analysis.

2. **Conversation Start**: Initiate the conversation using the provided prompt template.

3. **Chat Flow**: Engage in a conversation with the chatbot. The Chains component manages the flow and context.

4. **Memory Preservation**: The Memory component stores context for coherent responses throughout the conversation.

5. **PDF Analysis**: The PDF is chunked, and embeddings are created using the OpenAI Text-Embedding-Ada-002 model. These embeddings are stored in the FAISS vector database for efficient retrieval.

## Dependencies

- OpenAI GPT-3.5 Turbo
- Langchain
- FAISS (for Vector Database)
- OpenAI Text-Embedding-Ada-002



Feel free to reach out for any questions or improvements! Happy chatting!
