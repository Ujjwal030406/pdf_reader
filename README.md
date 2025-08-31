# Multi-PDF-s 📚 ChatApp AI Agent 🤖

Meet MultiPDF Chat AI App! 🚀 Chat seamlessly with Multiple PDFs using LangChain, Google Gemini Pro & FAISS Vector DB with seamless Streamlit Deployment. Get instant, accurate responses from Google Gemini language models. 📚💬 Transform your PDF experience now! 🔥✨

---

## 📝 Description

The Multi-PDF's Chat Agent is a **Streamlit-based web application** designed to facilitate interactive conversations with multiple documents. The app allows users to upload PDFs, extract text information, and train a chatbot using the extracted content. You can then have real-time conversations with the chatbot — just like chatting with your documents!

## 🎯 How It Works

![MultiPDF Chat App Diagram](img/Architecture.jpg)

1. **PDF Loading** → The app reads multiple PDF documents and extracts their text content.
2. **Text Chunking** → Extracted text is divided into smaller chunks for better processing.
3. **Embeddings** → A language model generates embeddings (vector representations) of these chunks.
4. **Similarity Search** → When a user asks a question, FAISS retrieves the most relevant chunks.
5. **Response Generation** → The LLM (Gemini/GPT/etc.) generates answers grounded in the PDFs.

---

## ✨ Features

* **Multi-Document Conversational QA** — Chat with several PDFs at once.
* **Adaptive Chunking** — Sliding window technique for efficient RAG.
* **File Support** — PDF and TXT files supported.
* **LLM Flexibility** — Works with Google Gemini Pro, OpenAI GPT, Claude, LLaMA, etc.

---

## 🌟 Requirements

* `streamlit`
* `google-generativeai`
* `python-dotenv`
* `langchain`
* `PyPDF2`
* `faiss-cpu`
* `langchain_google_genai`

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Installation

Clone this repo:

```bash
git clone https://github.com/Ujjwal030406/pdf_reader.git
cd pdf_reader
```

Set up your Google API key from [Google MakerSuite](https://makersuite.google.com/app/apikey) by creating a `.env` file in the project root:

```
GOOGLE_API_KEY=your_api_key_here
```

Run the Streamlit app:

```bash
streamlit run chatapp.py
```

---

## 💡 Usage

1. Open the Streamlit app in your browser.
2. Upload one or more PDFs in the sidebar.
3. Click **Submit & Process** to prepare the documents.
4. Start chatting with your documents using natural language!

## 🙏 Credits

This project was **adapted and extended** from the original work by [Gurpreet Kaur Jethra](https://github.com/GURPREETKAURJETHRA) — [Multi-PDFs ChatApp AI Agent](https://github.com/GURPREETKAURJETHRA/Multi-PDFs_ChatApp_AI-Agent).
Special thanks for the excellent base implementation and architecture diagrams.
