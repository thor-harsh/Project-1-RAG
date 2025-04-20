## Project-1-RAG(LangChain-Text-QnA-Bot 🤖💬)

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
```

### Folder Structure
```bash
.
├── docs/
│   └── user-manual.txt        # Source document
├── main.py                    # Your chatbot code
├── .env                       # Store OpenAI API key here
```

### .env File Format
Create a .env file in the root directory and add your OpenAI API key:
```bash
OPENAI_API_KEY=your_openai_api_key_here
```

### How the Bot Works – Step by Step

1. Loads a text file using TextLoader
2. Splits it into manageable chunks using CharacterTextSplitter
3. Embeds those chunks using OpenAIEmbeddings()
4. Stores them in Chroma vector DB
5. Uses LangChain to retrieve the most relevant chunk
6. Sends it to OpenAI to get a natural language answer
7. Boom! 🎉 You get your answer in the CLI

### How to Run the Project
Just run the script:
```bash
python main.py
```
Then follow the CLI prompts:
1. Press [1] to ask a question
2. Press [2] to exit
3. Press x during a Q&A to go back to the main menu

### Example Interaction
```bash
MENU
====
[1]- Ask a question
[2]- Exit

Enter your choice: 1

Q: How do I reset the device?

A: To reset the device, hold the power button for 10 seconds...
-------------------------------------------------
```

**Note:** Before running the code, make sure you have a valid user-manual.txt inside the /docs folder.
You can replace it with any .txt file you want your bot to learn from.


**For help:** Open a pull request or create an issue – happy to help! 😁

What are you waiting for...? Jump into the code and start asking questions!
As usual, for any doubt or query – see you in the pull request section 😁😂
