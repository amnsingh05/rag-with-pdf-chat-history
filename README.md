# 📄 Conversational RAG with PDF Uploads & Chat History

A **Conversational Retrieval-Augmented Generation (RAG)** application built using **LangChain**, **Groq**, **ChromaDB**, **Hugging Face Embeddings**, and **Streamlit**.

Upload a PDF document, ask questions about its content, and continue the conversation with persistent chat history using unique session IDs.

---

## 🚀 Features

- 📄 Upload and process PDF documents
- 💬 Ask questions based on uploaded PDFs
- 🧠 Context-aware conversations with chat history
- 🔍 Semantic search using Chroma Vector Database
- 🤖 Fast inference with Groq (Llama 3.1)
- 📚 Hugging Face Sentence Transformers for embeddings
- 📝 Session-based conversations
- ⚡ Simple and interactive Streamlit interface

---

## 🖼️ Project Preview

### 🏠 Home Page


```markdown
![Home Page](photos\home_page.png)
```

---

### 💬 Question Answering

The chatbot retrieves relevant information from the uploaded PDF and generates accurate answers.

```markdown
![Question Answering](photos\question-answer1.png)
![Question Answering](photos\question-answer2.png)
```

---

### 🧠 Chat History

The application remembers previous conversations within the same session, enabling context-aware follow-up questions.

```markdown
![Chat History](photos\chat-history.png)
```

---

## 🏗️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Streamlit | Web Interface |
| LangChain | LLM Framework |
| Groq | LLM Inference |
| ChromaDB | Vector Database |
| Hugging Face | Text Embeddings |
| PyPDFLoader | PDF Processing |
| RecursiveCharacterTextSplitter | Document Chunking |
| RunnableWithMessageHistory | Chat Memory |
| dotenv | Environment Variables |

---

## 📂 Project Structure

```text
rag-with-pdf-upload/
│
├── photos/
│   ├── home_page.png
│   ├── question-answer1.png
│   └── question-answer2.png
│   └── chat-history.png
│
├── app.py
├── requirements.txt
├── .env
├── README.md
└── temp.pdf
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/amnsingh05/rag-with-pdf-upload.git
```

```bash
cd rag-with-pdf-upload
```

---

### 2️⃣ Create a Virtual Environment

**Windows**

```bash
python -m venv venv
```

Activate it

```bash
venv\Scripts\activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Create a `.env` File

```env
HF_TOKEN=your_huggingface_token
```

> **Note:** The Groq API Key is entered directly in the application UI.

---

### 5️⃣ Run the Application

```bash
streamlit run app.py
```

---

## 🔄 How It Works

```text
             Upload PDF
                  │
                  ▼
           PyPDFLoader
                  │
                  ▼
      Text Chunking (RecursiveCharacterTextSplitter)
                  │
                  ▼
     Hugging Face Embeddings
                  │
                  ▼
         Chroma Vector Store
                  │
                  ▼
     History Aware Retriever
                  │
                  ▼
        Groq (Llama 3.1)
                  │
                  ▼
      Context-Aware Response
                  │
                  ▼
      Chat History is Stored
```

---

## 💬 Example Questions

- What is the Transformer architecture?
- Summarize the uploaded paper.
- Explain self-attention in simple words.
- What problem does the paper solve?
- What are the encoder and decoder?
- What are the key contributions of the paper?
- Give a detailed summary.
- Explain positional encoding.

---

## ✨ Key Concepts Used

- Retrieval-Augmented Generation (RAG)
- Conversational RAG
- Context-Aware Retrieval
- Chat Memory
- Vector Embeddings
- Semantic Search
- Document Chunking
- Prompt Engineering
- Session-Based Conversations

---

## 📦 Dependencies

- streamlit
- langchain
- langchain-community
- langchain-classic
- langchain-chroma
- langchain-groq
- langchain-huggingface
- chromadb
- sentence-transformers
- pypdf
- python-dotenv

---

## 🚀 Future Improvements

- 📚 Multiple PDF support
- 💬 ChatGPT-style chat interface
- 📖 Source citations
- ⚡ Streaming responses
- 💾 Persistent vector database
- ☁️ Streamlit Cloud deployment
- 📥 Export conversation
- 🎨 Improved UI/UX
- 🌐 Multi-document retrieval

---

## 👨‍💻 Author

**Aman Singh**

**LinkedIn**  
https://linkedin.com/in/amnsingh0

**GitHub**  
https://github.com/amnsingh05

---

## ⭐ Support

If you found this project helpful, please consider giving it a **⭐ Star** on GitHub. It helps others discover the project and supports future development.

---