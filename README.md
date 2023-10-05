# Personal Chatbot using Llama 2

This repository contains code for a personal chatbot that utilizes Llama 2 for natural language processing. The chatbot is designed to answer questions about the owner's professional background, including education, certifications, projects, and achievements. It does so by analyzing a dataset provided in a PDF file.

## Prerequisites

Before using this chatbot, you need to set up a few things:

1. **Hugging Face API Key**: Replace the 'huggingface api key' with your actual Hugging Face API key in the code where the AutoTokenizer and AutoModelForCausalLM are instantiated.

2. **Data PDF**: Replace "/content/data.pdf" with the path to your dataset in the PyPDFLoader instantiation.

## How it Works

1. **Tokenization and Model Loading**: The chatbot tokenizes input questions and utilizes a pre-trained language model from Hugging Face for generating responses.

2. **Data Loading**: The chatbot loads and processes data from the provided PDF file. It extracts text from the PDF using a text splitter.

3. **Question Answering**: Given a user's question, the chatbot uses the loaded dataset to provide relevant answers.

4. **Conversation Memory**: The chatbot retains a conversation history, making it context-aware for answering follow-up questions.

## Usage

1. To interact with the chatbot, run the provided Jupyter Notebook (.ipynb) in your environment.

2. You can input questions and receive responses from the chatbot.

3. Use the "Clear LLM Memory" button to clear the chatbot's conversation history.

4. Use the "Update System Prompt" text box to change the system prompt used by the chatbot.

## Configuration

- You can configure the chatbot's behavior by modifying the system prompt and other parameters in the code.

- The system prompt defines the behavior and guidelines for the chatbot when answering questions.

## Dependencies

- This project relies on various Python libraries, including PyTorch, Transformers, Gradio, and LangChain. Ensure you have these dependencies installed in your environment.

## Acknowledgments

This project utilizes the Llama 2 model by Hugging Face.
