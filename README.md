
# 🚀 IntelliDocs: Your Intelligent Document Analyst[](http://localhost:8501/#intelli-docs-your-intelligent-document-analyst)

Unlock the knowledge within your documents. Upload, ask, and get intelligent answers instantly.

- Upload multiple document formats (PDF, DOCX, TXT)
- Process and analyze documents automatically
- Ask questions about your documents
- Get AI-generated answers using Groq's LLama 3 models
- Select from multiple LLM models with different capabilities
- Adjust response parameters (temperature, max tokens)
- View chat history

## Setup

1. Install the required packages:

```bash
pip install -r requirements.txt
```

2. Set up your environment variables:

Create a `.env` file in the project root with the following:

```
GROQ_API_KEY=your_groq_api_key
```

3. Run the application:

```bash
streamlit run app.py
```

## Usage

1. **Upload Documents**:

   - Use the sidebar to upload PDF, DOCX, or TXT files
   - Click "Process Documents" to analyze and store them
2. **Ask Questions**:

   - Type your question in the input field
   - Click "Submit Question" to get an answer
3. **Adjust Settings**:

   - Select different LLM models from the dropdown
   - Adjust temperature for more deterministic or creative responses
   - Change max tokens to control response length

## Project Structure

- `app.py`: Main Streamlit application
- `document_processor.py`: Utilities for processing documents
- `model_utils.py`: Functions for interacting with Groq API
- `requirements.txt`: Required Python packages
- `chroma_db/`: Directory for ChromaDB vector database

## Supported Document Formats

- PDF (`.pdf`)
- Microsoft Word (`.docx`)
- Plain Text (`.txt`)

## Supported LLM Models

The application supports various Groq LLM models, including:

- LLama 3 (8B, 70B)
- LLama 3.1 and 3.3
- Gemma 2
- LLama 4 (Preview)
- Mistral Saba
- And more

## Limitations

- Document processing may take time for large files
- Response quality depends on the selected model and document content
- Some document formats may not be parsed perfectly

## License

This project is open source and available for personal and commercial use.
