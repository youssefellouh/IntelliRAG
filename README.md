# IntelliRAG

IntelliRAG is a project focused on building an intelligent document management and question-answering system. It leverages OpenAI's language models, document loaders, and persistent vector storage to enable efficient information retrieval from a collection of documents.

## Features

- **Document Loading**: Supports loading and parsing PDFs from a specified directory.
- **Text Splitting**: Utilizes recursive text splitting for optimal document chunking.
- **Persistent Storage**: Integrates with ChromaDB for scalable and persistent storage of document embeddings.
- **Interactive Querying**: Allows users to input questions and receive answers based on the loaded document content.

## Technologies Used

- **Python**: Core programming language.
- **OpenAI API**: Used for generating responses and interacting with language models.
- **ChromaDB**: Manages vector storage for document embeddings.
- **LangChain**: Assists with document processing and text splitting.
- **PyPDF**: For reading and extracting text from PDFs.
- **dotenv**: Manages environment variables for secure API key handling.

## Project Structure

```
IntelliRAG/
|-- data/                       # Directory for storing PDF documents
|-- ask.py                      # Main script for querying the system
|-- load_and_process.py         # Script for loading and processing documents
|-- .env                        # Environment variables
|-- README.md                   # Project documentation
```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/youssefellouh/IntelliRAG.git
   cd IntelliRAG
   ```

2. **Create and activate a virtual environment**:
   ```bash
   python3 -m venv .env
   source .env/bin/activate  # On Windows use `.env\Scripts\activate`
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   Create a `.env` file and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

## Usage

1. **Prepare your documents**: Place your PDF files in the `data/` directory.

2. **Run the document loading script**:
   ```bash
   python load_and_process.py
   ```

3. **Query the system**:
   ```bash
   python ask.py
   ```
   Enter your question when prompted.

