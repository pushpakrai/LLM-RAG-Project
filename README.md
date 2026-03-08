
<div align="center">
  <h1>🧠 LLM RAG </h1>
  <h3>Retrieval-Augmented Generation Chatbot with Streamlit</h3>

  <p>
    <em>A simple yet powerful RAG application that lets you chat with your documents using modern LLMs.</em>
  </p>

  <p>
    <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
    <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit"/>
    <img src="https://img.shields.io/badge/LangChain-00BFFF?style=for-the-badge&logoColor=white" alt="LangChain"/>
    <img src="https://img.shields.io/badge/ChromaDB-FF6F61?style=for-the-badge&logoColor=white" alt="Chroma"/>
  </p>
</div>

---

### ✨ Features

- 📄 Upload PDFs or text files from your device
- 🔍 Intelligent document chunking & embedding
- 🗄️ Vector storage with Chroma
- 🔄 Re-ranking for improved answer quality
- 💬 Conversational interface powered by OpenAI / Groq / local models
- 🔒 Fully local processing possible

### 🛠️ Tech Stack

- **UI** → Streamlit  
- **RAG Framework** → LangChain / LlamaIndex  
- **Embeddings** → all-MiniLM-L6-v2 (or OpenAI)  
- **Vector Store** → Chroma  
- **LLM** → GPT-3.5-turbo / Groq / Ollama (configurable via .env)  
- **Python** → 3.10+

### 📂 Project Structure

```
LLM-RAG-/
├── src/                # Main application code
│   └── app.py          # Streamlit entry point
├── assets/             # Images, icons, custom CSS
├── data/
│   └── wiki/           # Sample documents / your files
├── requirements.txt
├── README.md
└── .env.example        # (create this if missing)
```

### 🚀 Quick Start

1. Clone the repository
```bash
git clone https://github.com/pushpakrai/LLM-RAG-.git
cd LLM-RAG-
```

2. Create virtual environment & install dependencies
```bash
python -m venv venv
source venv/bin/activate          # Windows → venv\Scripts\activate
pip install -r requirements.txt
```

3. Set up environment variables  
   Create a `.env` file in the root:
   ```
   OPENAI_API_KEY=sk-...
   # OR
   GROQ_API_KEY=gsk_...
   # Optional: MODEL_NAME=gpt-3.5-turbo or llama3-70b-8192
   ```

4. Run the application
```bash
streamlit run src/app.py
```

Open → http://localhost:8501

---

### 💡 Tips

- Put your documents in `data/` or upload them through the UI
- First run will download embedding model (~80–100 MB)
- For faster/larger models → use Groq or local Ollama

### 📌 Future Improvements (Ideas)

- Multi-file / folder upload
- Persistent vector store
- Chat history saving
- Advanced prompt engineering
- Evaluation metrics (RAGAS / TruLens)

---

<div align="center">
  <p>⭐ If this project helps you — please give it a star!</p>
  <p>Contributions, issues, and feature requests are welcome 🚀</p>
</div>
the instructions.

Let me know if you want to add screenshots, a demo GIF, deployment instructions (Streamlit Cloud / Hugging Face), or anything else!
