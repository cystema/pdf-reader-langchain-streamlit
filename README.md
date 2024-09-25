# Interactive PDF Reader with Conversational AI

This application allows users to upload a PDF document and ask questions about its content through a conversational AI interface. The AI uses document embeddings and a conversational retrieval chain to provide intelligent answers based on the contents of the uploaded PDF.

## Features

- PDF Upload & Processing: Users can upload a PDF document, which is processed by an AI model that extracts and indexes the content for question-answering.
- Conversational AI: Leveraging LangChain's conversational retrieval chain, users can ask questions about the PDF, and the AI will retrieve relevant sections to generate an appropriate response.
- Chat Interface: A user-friendly chat interface for interacting with the AI.

## How It Works

- Upload a PDF: Use the provided file uploader to select the PDF document.
- Process the PDF: Once uploaded, click the "Process" button to extract and index the content.
- Ask Questions: Type your question in the input box, and the AI will retrieve relevant information from the PDF to answer your question.
- Review Results: The app will display both the conversational response and the related pages from the PDF.

## Technologies Used

- Streamlit: For the web application interface.
- LangChain: For building conversational chains and document embeddings.
- HuggingFace Embeddings: To create text embeddings from the document for better retrieval accuracy.
- Chroma: As a vector store for indexing the document embeddings.
- PyPDF2: For reading and parsing PDF files.

## Installation

To run this app locally, follow these steps:

- Clone this repository:

```bash
git clone https://github.com/cystema/pdf-reader-langchain-streamlit.git
cd pdf-reader-langchain-streamlit.git
```

- Create a virtual environment and activate it:

```bash
python -m venv venv
source venv/bin/activate 
```

- Install the required dependencies:

```bash
pip install -r requirements.txt
```

- Run the Streamlit app:

```bash
streamlit run app.py
```