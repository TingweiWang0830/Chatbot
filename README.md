# 💬 Chat with Your PDFs (Multi-LLM Support)

A local AI-powered chatbot that allows you to query and interact with your PDF documents using powerful open-source language models like **Gemini**, **OpenAI**, and **Ollama** (e.g., DeepSeek-Coder, Mistral). Perfect for summarization, question-answering, and deep document analysis — all on your own machine.

## 🚀 Features

- 📄 Upload and query PDF files
- 🧠 Use multiple local or cloud-based LLMs (Gemini, OpenAI, Ollama)
- 🔍 Accurate retrieval using state-of-the-art embedding models
- 💾 FAISS-based vector store for fast semantic search
- 🎛️ Easy model switching via dropdown
- 🖥️ Built with Streamlit for a clean, user-friendly interface
- 🔒 100% local option (via Ollama) to keep your data private

## 🛠 Tech Stack

- `Python` · `LangChain` · `FAISS` · `Streamlit`
- `Ollama`, `Google Generative AI`, `OpenAI API`
- PDF parsing and vector storage

## 📊 Recommended Model & Embedding Combinations

| LLM              | Embedding Model        | Use Case                        |
|------------------|------------------------|----------------------------------|
| Gemini 2.0 Flash | `models/embedding-001` | Fast cloud-based Q&A            |
| OpenAI GPT-3.5   | `text-embedding-3-small`| High-quality cloud Q&A         |
| DeepSeek-Coder   | `mxbai-embed-large`    | Best fully local PDF analysis   |
| Mistral          | `nomic-embed-text`     | Lightweight local setup         |

## 💻 Local Setup

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/chat-with-pdf-LLM.git
cd chat-with-pdf-LLM

```
### 2. Install Requirements
```bash
pip install -r requirements.txt

```
### 3. Pull Ollama Models (optional)
```bash
ollama pull Malicus7862/deepseekcoder-6.7b-jarvis-gguf
ollama pull mxbai-embed-large

```
### 4. Launch App
-For Ollama-based local models:
```bash
streamlit run chat_with_pdf_ollama_with_history.py
```
-For Gemini:
```bash
streamlit run chat_with_pdf_gemini.py
```
-For OpenAI:
```bash
streamlit run chat_with_pdf_openai.py

```
Use Cases:
Academic paper analysis
Legal contract review
Business reports summarization
Private file Q&A without uploading to cloud

👤 Author
Tingwei Wang
🎓 M.S. in Information Systems, Johns Hopkins University

