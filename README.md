# GenAI_Project2_Multi_PDF_Reader

# Gemini PDF Chatbot 🤖

This application enables users to interact with uploaded PDF documents using Google's Gemini 1.5 Flash model.
Users can ask questions related to the content of the PDFs, and the chatbot provides detailed answers, retrieving relevant information from the documents. 
If the answer isn't present in the document, the chatbot responds accordingly.

## Features

- **PDF Upload**: Users can upload multiple PDF files.
- **Text Chunking**: Text from the PDF is split into manageable chunks for processing.
- **Google Gemini AI**: Integrated with the Google Generative AI model (Gemini 1.5 Flash) for answering questions based on the content of the PDFs.
- **Vector Storage**: Uses FAISS for storing and searching through vectorized chunks of text.
- **Interactive Chat**: Users can engage in a conversational format to query the PDF content.

## Technology Stack

- **Streamlit**: Frontend framework for user interaction.
- **LangChain**: For managing text processing and question-answering chains.
- **FAISS**: Vector database for efficient similarity searches.
- **Google Generative AI (Gemini)**: Provides the model for generating responses.
- **PyPDF2**: Library for reading PDFs.
- **Python**: Core programming language.

## Installation

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Create a `.env` file and add your Google API key:
   ```bash
   GOOGLE_API_KEY=your_google_api_key
   ```

## Usage

1. Run the Streamlit application:
   ```bash
   streamlit run app.py
   ```

2. Upload your PDF documents using the sidebar and process them.
3. Interact with the chatbot in the main window by asking questions related to the uploaded PDFs.

## Example Use Case

- **Upload PDFs**: Upload any set of documents for analysis.
- **Ask a Question**: "What is the total amount on the invoice?" or "Tell me about section 2 of the document."

## Notes

- **Chat History**: You can clear the chat history by clicking the 'Clear Chat History' button in the sidebar.
- **Detailed Responses**: If the chatbot finds relevant information in the context, it will generate detailed responses. Otherwise, it will notify the user that the answer is not available in the context.

Feel free to modify the content to meet your specific needs!
