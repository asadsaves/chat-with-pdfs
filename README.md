# Chat with PDFs

Welcome to the **Chat with PDFs** repository! This project is a Python-based application that allows users to interact with the content of multiple PDF documents using natural language queries. The app intelligently retrieves relevant information from the PDFs based on user questions and responds with contextually accurate answers.

## Features

- Upload multiple PDF files for processing.
- Ask questions in natural language and get relevant responses from the PDF content.
- Utilizes advanced language models for processing and response generation.
- Easy-to-use interface built with Streamlit.

## How It Works
![Chat with PDFs](https://github.com/asadsaves/chat-with-pdfs/blob/main/PDF-LangChain.jpg?raw=true)

The application follows these steps to process user queries:

1. **PDF Loading**: Users upload multiple PDFs, and the app extracts text from the documents.
2. **Text Chunking**: The extracted text is split into smaller chunks for efficient processing.
3. **Language Model**: A language model generates embeddings (vector representations) for each text chunk.
4. **Similarity Matching**: User queries are compared with the text chunks to identify the most semantically similar chunks.
5. **Response Generation**: The language model generates an appropriate response based on the most relevant text chunks.

## Installation

Follow these steps to set up the application on your local machine:

1. Clone the repository:

   ```bash
   git clone https://github.com/asadsaves/chat-with-pdfs.git
   ```

2. Navigate to the project directory:

   ```bash
   cd chat-with-pdfs
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Obtain an OpenAI API key from [OpenAI](https://openai.com) and add it to the `.env` file in the root directory of the project:

   ```bash
   OPENAI_API_KEY=your_secret_api_key
   ```

## Usage

1. Ensure that all dependencies are installed and the API key is set.
2. Launch the application using Streamlit:

   ```bash
   streamlit run app.py
   ```

3. The application will open in your default web browser. Follow the instructions to upload PDF documents.
4. Ask questions about the uploaded PDFs using the chat interface, and the app will return relevant responses.

## Example

1. **Upload PDFs**: Add multiple PDFs through the provided file upload interface.
2. **Ask Questions**: Type questions like "What is the main topic of the second document?" or "Summarize the key points in Chapter 3."
3. **Receive Answers**: The app will retrieve the most relevant information from the PDFs and display an answer.

## Dependencies

- Python 3.7+
- Streamlit
- OpenAI API
- Other dependencies listed in `requirements.txt`

## Contributing

This project is primarily for educational purposes and is based on a project tutorial. Feel free to fork the repository and make changes according to your needs. Contributions are welcome for improving features and usability.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

Thank you for using **Chat with PDFs**! If you encounter any issues or have feature requests, feel free to open an issue on GitHub.
