⚖️ LawBuddy – AI Legal Advisory Chatbot for Indian Law
Your Personal AI Legal Guide, Powered by LLMs + LangChain + RAG Pipeline
<p align="center"> <img src="https://img.shields.io/badge/Project-LawBuddy-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/AI%20Chatbot-Legal-brightgreen?style=for-the-badge&logo=semantic-web" /> <img src="https://img.shields.io/badge/Made%20With-Python-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/Framework-LangChain-orange?style=for-the-badge&logo=apache-spark" /> <img src="https://img.shields.io/badge/UI-Streamlit-red?style=for-the-badge&logo=streamlit" /> </p>
🧾 Overview

LawBuddy is an advanced AI-powered Legal Advisory Chatbot designed to simplify Indian Law for students, citizens, lawyers, and anyone seeking legal clarity.

Built using:

Llama-7B Chat (Meta)

LangChain RAG (Retrieval-Augmented Generation)

FAISS Vector Search

Streamlit UI

LawBuddy enables you to chat with your legal documents — IPC, CrPC, Constitution, Cyber Law, Consumer Rights, and more.

⭐ Key Features
🗣️ Natural Legal Conversations

Ask questions like:

“What are my rights if a shop refuses a refund?”
“How do I file an FIR?”
“What is Section 420 of IPC?”

📚 Custom Legal Knowledge

Add your own PDFs to the dataset/ folder — LawBuddy learns automatically.

🧠 RAG-Powered Accuracy

Combines vector search + LLM for highly relevant legal answers.

⚡ Fast & Local

Runs 100% locally — no API cost, no internet dependency.

💻 Clean Streamlit UI

Simple and modern user interface.

🛠️ Tech Stack
Component	Technology
LLM	Llama-7B-Chat
Framework	LangChain
Vector DB	FAISS
Frontend UI	Streamlit
Embeddings	HuggingFace Transformers
Backend	Python
🧩 RAG Architecture (Premium Diagram)
          ┌───────────────────────────┐
          │      User Question        │
          └─────────────┬─────────────┘
                        │
                        ▼
              ┌──────────────────┐
              │   Retriever       │
              │ (FAISS Vector DB) │
              └─────────┬────────┘
                        │
           Relevant Legal Chunks
                        │
                        ▼
       ┌────────────────────────────────┐
       │         Llama-7B-Chat          │
       │ (Generates Final Legal Answer) │
       └────────────────────────────────┘
                        │
                        ▼
          ┌───────────────────────────┐
          │      Streamlit UI         │
          └───────────────────────────┘

📁 Project Structure
LawBuddy/
│── app.py                 # Main Streamlit UI
│── ingest.py              # Build vector DB from PDFs
│── requirements.txt       
│── utils.py               # Helper functions
│── dataset/               # Add your PDFs here
│── vectorstore/           # Auto-generated embeddings
│── README.md
│── LICENSE

🔧 Installation
git clone https://github.com/Anmolkankarwal/LawBuddy.git
cd LawBuddy
python -m venv venv
venv\Scripts\activate     # Windows
pip install -r requirements.txt

🚀 Usage
1️⃣ Add legal PDFs

Place your documents in:

/dataset

2️⃣ Build vector database
python ingest.py

3️⃣ Run the chatbot
streamlit run app.py


Open: http://localhost:8501

💬 Example Conversations
User:

“What is Section 420 of IPC?”

LawBuddy:

Section 420 deals with cheating and dishonestly inducing delivery of property. The punishment may include imprisonment up to 7 years and a fine.

User:

“How to file a consumer complaint?”

LawBuddy:

Under the Consumer Protection Act 2019, you can file complaints online via the E-Daakhil portal or at your district consumer forum.

🌟 Future Enhancements

🎙️ Voice chat (speech-to-text + TTS)

📑 Automated legal document drafting

🧑‍⚖️ Case-law integration (Supreme / High Court)

🌐 Hindi & regional languages

🔗 Multimodal legal search

🔗 Connect With Me




📚 References

LangChain Docs

FAISS Vector Search

HuggingFace Transformers

Streamlit Documentation

✍️ Author

Anmol Kankarwal
📅 2025
