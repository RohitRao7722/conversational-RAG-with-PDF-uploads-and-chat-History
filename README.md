# conversational RAG with PDF uploads and chat History

This project implements a Conversational RAG (Retrieval-Augmented Generation) system using Langchain, enabling users to upload PDF files and ask questions about their contents. It integrates with Groq for large language model processing and stores chat history to provide context-aware answers.

## Features

- **PDF Upload**: Allows multiple PDFs to be uploaded for context-based querying.
- **Chat History**: Maintains a session-based chat history for continuous context in conversations.
- **Retrieval-Augmented Generation**: Uses documents from uploaded PDFs and chat history for answering questions.
- **Groq Integration**: Powered by Groq's API to run the model efficiently.

## Requirements

- Python 3.7+
- Required libraries:
  - `streamlit`
  - `langchain`
  - `langchain_huggingface`
  - `langchain_chroma`
  - `langchain_community`
  - `python-dotenv`
  - `PyPDF2`
  - `huggingface_hub`

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/conversational-rag-pdf.git
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your environment file `.env` to store your Hugging Face token:**

   ```
   HF_token=your_huggingface_token_here
   ```

4. **Start the Streamlit app:**

   ```bash
   streamlit run app.py
   ```

## Usage

1. **Upload PDFs:** Use the file uploader to upload one or more PDF files.
2. **Enter Groq API Key:** Input your Groq API key to power the language model.
3. **Ask Questions:** Type your question in the input box. The system will use the uploaded PDFs and chat history to generate answers.
4. **View Chat History:** See the conversation history along with the assistant’s responses.

## License

This project is licensed under the MIT License. 
