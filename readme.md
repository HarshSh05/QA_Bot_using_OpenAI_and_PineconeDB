
# RAG QA Bot

This repository contains the implementation of a **Retrieval Augmented Generation (RAG)** model for a Question Answering (QA) bot using **OpenAI API** and **Pinecone DB**. The project showcases a robust pipeline for retrieving relevant documents and generating context-aware answers using GPT models.

## Project Description

The QA bot is designed for businesses to answer user queries intelligently by leveraging a combination of retrieval and generation techniques:

1. **Document Embedding**: Converts documents into vector representations using OpenAI's `text-embedding-ada-002`.
2. **Vector Search**: Stores and retrieves document embeddings using Pinecone, a vector database.
3. **Response Generation**: Uses OpenAI's GPT model to generate natural language answers by combining user queries and retrieved document content.

## Features

- Document retrieval using Pinecone DB.
- OpenAI GPT-powered response generation.
- Real-time QA with meaningful and context-aware answers.
- Configurable and easy to extend for various business use cases.

## Prerequisites

- Python 3.7 or later
- OpenAI API Key
- Pinecone API Key and Environment
- Required Python libraries (see `requirements.txt`)

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/HarshSh05/QA_Bot_using_OpenAI_and_PineconeDB
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set environment variables for OpenAI and Pinecone API keys:
   ```bash
   export OPENAI_API_KEY="your_openai_api_key"
   export PINECONE_API_KEY="your_pinecone_api_key"
   export PINECONE_ENV="your_pinecone_environment"
   ```

4. Run the Colab notebook:
   - Open `main.ipynb` in Google Colab.
   - Follow the instructions in the notebook to set up the Pinecone index, add documents, and run queries.

## Example Usage

1. Add your documents to the Pinecone database.
2. Query the bot, e.g., `"What services do you offer?"`
3. Get a meaningful response like:
   ```
   "We offer a range of services, including cloud computing, AI solutions, and GDPR/CCPA-compliant offerings."
   ```
