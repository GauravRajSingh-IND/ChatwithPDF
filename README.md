# Chat with PDF - Document Question Answering System

Welcome to the **Chat with PDF** repository! This project allows users to upload PDF documents and interact with them using a Question-Answering system powered by OpenAI's language models. It uses **LangChain** for document processing and integrates **OpenAI's GPT** for generating responses.

## Features

- **Upload PDF files**: Upload any PDF document to the system.
- **Document Processing**: The document is processed and split into chunks for easier querying.
- **Ask Questions**: Users can ask questions related to the content of the PDF, and the system provides answers based on the document.
- **Source Citation**: The system provides the source of the information used to generate the answer.

## Installation

### Prerequisites

- Python 3.8 or higher
- Git
- API keys for OpenAI (you can add your keys in a `.env` file)

### Steps to Set Up

1. **Clone the repository**:
    ```bash
    git clone https://github.com/GauravRajSingh-IND/ChatwithPDF.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd ChatwithPDF
    ```

3. **Install dependencies**:
    It’s recommended to use a virtual environment to manage the dependencies.
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # For macOS/Linux
    venv\Scripts\activate     # For Windows
    ```

    Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:
    Create a `.env` file in the root directory of the project and add your OpenAI API key:
    ```
    OPENAI_API_KEY=your-openai-api-key
    ```

    > **Note**: Make sure to replace `your-openai-api-key` with your actual OpenAI API key. Keep the `.env` file private and do not push it to GitHub.

5. **Run the Streamlit app**:
    After setting up everything, you can launch the app with Streamlit:
    ```bash
    streamlit run app.py
    ```

    The app will be available at `http://localhost:8501`.

## Usage

1. **Upload a PDF**: Use the file uploader to upload your PDF document.
2. **Configure Document Settings**: You can adjust settings like chunk size, chunk overlap, and model temperature in the sidebar.
3. **Ask Questions**: Enter any question related to the document, and the system will provide an answer based on the document content.

## Project Structure


## Troubleshooting

### Common Errors:

1. **OpenAI API Key Missing**: Ensure you’ve set the `OPENAI_API_KEY` in the `.env` file.
2. **File Processing Error**: Ensure the uploaded PDF is not corrupted and is a valid document.
3. **Streamlit App Not Launching**: Ensure all dependencies are installed and try running the app again.

## Contributing

We welcome contributions! If you have suggestions or improvements, feel free to open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- **LangChain**: For handling document processing and question-answering workflows.
- **OpenAI**: For providing GPT-based models for the Q&A system.
- **Streamlit**: For creating the interactive web interface.

---

Happy coding! 🚀
