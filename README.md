# Financial Report Q&A Bot

## 🚀 Live Demo

Try the application here: https://financial-report-by-soham.streamlit.app/

A Retrieval-Augmented Generation (RAG) application that lets users upload PDF documents and ask questions about their contents.

## Features

- Upload financial reports and other PDF documents
- Extract text and split it into smaller chunks
- Generate embeddings and store them in ChromaDB
- Retrieve relevant text chunks using semantic search
- Ask questions and generate answers based on retrieved context
- View the source chunks used to generate each answer
- Choose between supported AI models, including GPT-4o mini, GPT-4o, and Gemini

## Tech Stack

- **Python** — application logic
- **Streamlit** — user interface
- **LangChain** — document chunking and retrieval
- **LiteLLM** — interface for supported language models
- **ChromaDB** — vector storage and similarity search
- **Hugging Face Sentence Transformers** — local embeddings
- **pdfplumber** — PDF text extraction

## How It Works

1. Upload a PDF document.
2. Extract text from the PDF.
3. Split the text into smaller chunks.
4. Generate embeddings and store the chunks in ChromaDB.
5. Retrieve relevant chunks for the user's question.
6. Send the retrieved context to the selected language model.
7. Display the answer and source chunks.

## Run Locally

Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
cd YOUR_REPOSITORY_FOLDER
```

Create and activate a virtual environment, then install dependencies:

```bash
python -m venv .venv
```

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

Start the application:

```bash
streamlit run app.py
```

## API Keys

The selected language model requires its corresponding API key. Configure API keys securely through environment variables or Streamlit secrets. Do not commit API keys to GitHub.

## Deployment

The application can be deployed using Streamlit Community Cloud. Deployment instructions and a live demo link will be added when available.

## Project Attribution

This project is based on an existing Financial Report Q&A Bot repository. Original authorship, attribution, and licensing should be preserved as required by the original project license.
