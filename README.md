
🧠 RAG-Powered Chatbot with LangChain & Streamlit
Welcome to your Retrieval-Augmented Generation (RAG) chatbot! This project leverages LangChain, Streamlit, and Groq to create an intelligent assistant that can answer questions based on the content of a PDF document.

🚀 Features
Retrieval-Augmented Generation (RAG): Combines LLM reasoning with document retrieval for accurate, up-to-date answers.

LangChain Integration: Modular, extensible, and easy to adapt to new data sources or models.

PDF Knowledge Base: Upload a PDF and ask questions about its contents.

Streamlit UI: Clean, interactive chat interface for seamless user experience.

Groq LLM Support: Fast, efficient inference for real-time conversation.

📦 Requirements
Python 3.8+
pipenv
A Groq API Key

🔧 Installation
Clone the repository:
bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
Install dependencies with pipenv:

bash
pipenv install
pipenv shell
Set your Groq API key:

Create a .env file in the project root

▶️ Usage
Run the chatbot with Streamlit:

streamlit run ph1.py
Open the provided local URL in your browser to interact with the chatbot.

📝 How It Works
Document Loading: The app loads and splits your PDF into chunks.
Vector Store: Embeddings are created using HuggingFace models and stored for fast retrieval.
RAG Pipeline: User questions are matched to relevant document chunks, and the LLM (via Groq) generates answers using both the retrieved context and its own knowledge.
Chat History: All interactions are displayed for context and continuity.

📂 Project Structure
text
├── ph1.py                # Main Streamlit chatbot app
├── reflexion.pdf         # Your knowledge base PDF
├── Pipfile               # pipenv dependency file
├── Pipfile.lock
├── .env                  # (optional) API keys and secrets
└── README.md
