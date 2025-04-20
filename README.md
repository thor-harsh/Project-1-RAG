# Project-1-RAG  
# LangChain-Text-QnA-Bot 🤖💬

**In this project, we’re building a _Text QnA Bot_ using LangChain + OpenAI + ChromaDB!**  
**This bot reads a user manual (or any `.txt` document), breaks it into smart chunks, turns it into embeddings, and then uses those to answer your queries.**  
**It's a basic, yet super cool way to create your own chatbot for any document!**

---

### 📚 About the Project

This project uses **LangChain** (an awesome library for LLM apps) and connects it with **OpenAI** (GPT-3.5 Turbo in this case) to build a document-based question-answering bot.  
You provide it with a text file (like a user manual), and it becomes your helpful assistant that can answer questions based on that file. Magic, right? ✨

---

### 🧠 What Tech Are We Using?

- **LangChain** – To manage the prompt chain and embeddings  
- **OpenAI** – For chatting magic  
- **ChromaDB** – A fast, lightweight vector store  
- **dotenv** – For storing your API keys securely  
- **colorama** – To make terminal output colorful and clean  

---

### 🛠️ Dependencies

Install the required packages using pip:

```bash
pip install langchain langchain-openai chromadb python-dotenv colorama

📂 Folder Structure
```bash
.
├── docs/
│   └── user-manual.txt        # Source document
├── main.py                    # Your chatbot code
├── .env                       # Store OpenAI API key here
