# PDF Chatbot

A Streamlit application that enables users to upload multiple PDF files and interact with the content through a conversational interface. It employs the Retrieval-Augmented Generation (RAG) algorithm via FAISS and Google's Generative Pre-trained Transformer for responsive and context-aware answers.

## Features

- Upload multiple PDF documents for processing.
- Extract text from the PDF files using PyPDF2.
- Split the text into manageable chunks for better context capturing.
- Create a FAISS index of embeddings for efficient similarity search.
- Utilize Google's Gemini LLM Model for generating responses to user queries.

![image](https://github.com/AnasNasim12/ChatWithPDF/assets/106335309/c1e754a6-317c-4b37-ab4d-e074a8806629)


## Installation

1. Clone this repository to your local environment.
2. Ensure that you have Python installed on your machine.
3. Install the necessary Python packages using:
```
pip install -r requirements.txt
```
4. You must have a `.env` file containing your `GOOGLE_API_KEY` for the Gemini LLM Model.

## Usage

1. Start the Streamlit app:
```
streamlit run chatpdf.py
```
2. Open the Streamlit application in your browser.
3. Use the sidebar to upload PDF files by clicking on the "Upload your PDF Files" button.
4. Once uploaded, click "Submit & Process" to index the content of the PDFs.
5. After processing, ask a question in the text input field to get responses based on the PDF content.

## Generative AI exploratory projects using Gemini
This repo also includes other simple projects that include utilization of the gemini-vision model, and a basic QnA system with a memory storage system.

## Credits

- [Streamlit](https://streamlit.io/) - For creating the web application.
- [PyPDF2](https://pypdf2.readthedocs.io/en/latest/) - For PDF text extraction.
- [LangChain](https://github.com/forensic-architecture/langchain) - For text splitting and chaining logic.
- [FAISS](https://github.com/facebookresearch/faiss) - For efficient similarity search.
- [Google GenerativeAI](https://pypi.org/project/google-generativeai/) - For embedding generation and conversational model.
