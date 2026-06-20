<div align="center">
  <h1>🏥 AI Healthcare Assistance Chatbot</h1>
  <p><strong>Intelligent RAG chatbot that answers health-related questions from uploaded medical PDFs using Google Gemini AI and FAISS vector search.</strong></p>

  <p>
    <a href="LICENSE">
      <img src="https://img.shields.io/github/license/SohaibKhaliq/AI-Healthcare-Assitance-Chatbot?style=flat-square&color=blue" alt="License"/>
    </a>
    <a href="https://github.com/SohaibKhaliq/AI-Healthcare-Assitance-Chatbot/stargazers">
      <img src="https://img.shields.io/github/stars/SohaibKhaliq/AI-Healthcare-Assitance-Chatbot?style=flat-square&color=yellow" alt="Stars"/>
    </a>
    <img src="https://img.shields.io/badge/python-3.9+-blue?style=flat-square&logo=python" alt="Python"/>
    <img src="https://img.shields.io/badge/Google_Gemini-GenAI-blue?style=flat-square&logo=google" alt="Gemini"/>
    <img src="https://img.shields.io/badge/FAISS-Vector%20Search-green?style=flat-square" alt="FAISS"/>
    <img src="https://img.shields.io/badge/Streamlit-UI-red?style=flat-square&logo=streamlit" alt="Streamlit"/>
  </p>
</div>

## 📖 Overview

AI Healthcare Assistance Chatbot uses **Retrieval-Augmented Generation (RAG)** to answer health-related queries based on medical PDF documents. Upload medical PDFs, the system extracts text, creates vector embeddings via Google Generative AI, stores them in FAISS, and answers questions using Gemini Pro.

### How It Works

1. **Upload PDFs** → Medical documents are stored in `LLM_DB/`
2. **Text Extraction** → PDF text extracted via pdfplumber
3. **Embeddings** → Text chunked and embedded via Google Generative AI
4. **Vector Store** → FAISS index for similarity search
5. **Q&A** → Questions matched against documents, answered by Gemini Pro

## 🚀 Quick Start

```bash
git clone https://github.com/SohaibKhaliq/AI-Healthcare-Assitance-Chatbot.git
cd AI-Healthcare-Assitance-Chatbot
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
# Create .env with: GOOGLE_API_KEY=your_key_here
streamlit run app.py
```

## 📄 License

MIT
