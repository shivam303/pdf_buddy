# 📄 DocuBuddy - PDF Chatbot

DocuBuddy is a powerful and intuitive chatbot application that allows you to have interactive conversations with your PDF documents. Simply upload a PDF, and DocuBuddy, powered by advanced language models, will answer your questions about its content.

## ✨ Features

- **Interactive PDF Chat**: Ask questions and get answers from your PDF documents in a conversational way.
- **OpenAI Integration**: Utilizes OpenAI's powerful language models for accurate and context-aware responses.
- **Easy to Use**: Simple and user-friendly interface for a seamless experience.
- **Secure**: Your API key and document content are handled securely.

## 🚀 Local Installation and Setup

Follow these steps to run DocuBuddy on your local machine:

### 1. Clone the Repository

```bash
git clone https://github.com/shivam303/pdf_buddy.git
cd DocuBuddy
```

### 2. Create a Virtual Environment

It's recommended to use a virtual environment to manage dependencies:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows, use `.venv\Scripts\activate`
```

### 3. Install Dependencies

Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```

### 4. Run the Application

Launch the Gradio application with the following command:

```bash
python app_gradio.py
```

The application will be available at a local URL (e.g., `http://127.0.0.1:7860`).

## ☁️ Deploying to Hugging Face Spaces

Deploying DocuBuddy to Hugging Face Spaces is a straightforward process:

### 1. Create a Hugging Face Account

If you don't have one, create a free account at [huggingface.co](https://huggingface.co/).

### 2. Create a New Space

- Click on your profile picture and select **"New Space"**.
- Choose a name for your space (e.g., `DocuBuddy`).
- Select **"Gradio"** as the SDK.
- Choose **"Public"** for visibility.

### 3. Upload Files

Upload the following files to your Hugging Face Space:

- `app_gradio.py`
- `requirements.txt`

### 4. Deploy

Hugging Face will automatically deploy your application. You can access it at `https://huggingface.co/spaces/your-username/your-space-name`.

## Usage

1.  **Enter Your OpenAI API Key**: Paste your OpenAI API key in the designated field.
2.  **Upload a PDF**: Click the "Upload PDF" button and select a PDF file from your computer.
3.  **Ask Questions**: Once the PDF is processed, you can start asking questions in the chat interface.

## Dependencies

- `gradio`
- `langchain`
- `langchain-community`
- `unstructured[pdf]`
- `sentence-transformers`
- `openai`
- `tiktoken`
- `chromadb`
- `python-dotenv`
- `pyocr`
