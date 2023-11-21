
# Amazon Ecommerce Chatbot with Google Palm

## Overview

This project implements a chatbot for an Amazon Ecommerce FAQ using the Google Palm language model and a FAISS vector database for document retrieval. The chatbot is designed to answer user queries based on a pre-existing FAQ dataset.

## Project Components

### Google Palm Language Model (LLM)

The chatbot utilizes the Google Palm language model for natural language understanding. The model is configured with a specific temperature to control the level of randomness in the generated responses.

### Vector Database

The FAQ dataset is loaded and processed to create a FAISS vector database. This database is used for efficient document retrieval during user queries.

### RetrievalQA Chain

The RetrievalQA chain is constructed using the Google Palm LLM, the FAISS vector database retriever, and a prompt template. This chain is responsible for generating answers to user queries based on the context provided in the FAQ dataset.

## Getting Started

To run the chatbot locally, follow these steps:

1. Install the required dependencies:

    ```bash
    pip install langchain streamlit python-dotenv
    ```

2. Set up your environment variables:

    Create a file named `.env` in the project directory and add your Google API key:

    ```dotenv
    GOOGLE_API_KEY=your_google_api_key
    ```

3. Run the Streamlit app:

    ```bash
    streamlit run app.py
    ```

4. Open your browser and go to [http://localhost:8501](http://localhost:8501) to interact with the chatbot.

## Usage

1. Click the "Create Knowledgebase" button to initialize the vector database.
2. Enter your questions in the text input and receive answers from the chatbot.

## Project Structure

- `app.py`: Streamlit app script for user interaction.
- `langchain_helper.py`: Helper functions for creating the vector database and constructing the RetrievalQA chain.
- `faiss_index`: Folder containing the serialized FAISS vector database.

## Dependencies

- [Streamlit](https://streamlit.io/)
- [Langchain](https://github.com/LuminosoInsight/langchain)
- [python-dotenv](https://github.com/theskumar/python-dotenv)

## About the Creator

**Parth dholakiya**

- Email: parthdholakiya180@gmail.com

## Acknowledgments

This project relies on the Google Palm language model and the Langchain library for efficient document retrieval. Special thanks to the creators of these tools.

Developed an e-commerce chatbot utilizing the Google Palm model and integrated Amazon e-commerce question and answer data.

![image](https://github.com/parthdholakiya/E-commerce-Chatbot-with-Google-Palm/assets/94167271/faa935d8-1d67-443d-b558-fe24c1a0dafd)
