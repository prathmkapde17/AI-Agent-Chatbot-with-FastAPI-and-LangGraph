# 🤖 AI Agent Chatbot – GenAI Application (Production Ready)

An **Agentic AI Chatbot** built with **LangGraph**, **FastAPI**, **Streamlit**, and **OpenAI/Groq LLMs**, featuring real-time search capabilities with Tavily, making it production deployable.

## 🚀 Features
- **LangGraph ReAct Agents** for dynamic reasoning
- **FastAPI backend** with Pydantic schema validation
- **Streamlit frontend** for interactive UI
- **Groq LLM / Meta LLaMA / Mistral / OpenAI GPT models** support
- Real-time **web search** via Tavily API
- **Modular architecture** for extension
- Deployable with **Uvicorn** or any ASGI server

---

## 📂 Project Layout

### Phase 1 – AI Agent Creation
1. Setup API Keys for Groq & Tavily
2. Initialize LLM & Tools
3. Build AI Agent with search tool functionality

### Phase 2 – Backend (FastAPI)
1. Define Pydantic Models (Schema Validation)
2. Setup AI Agent to process frontend requests
3. Run app & test endpoints in Swagger UI

### Phase 3 – Frontend (Streamlit)
1. Build UI with provider, model, system prompt, and query input
2. Connect Streamlit app with backend API

---

## 🛠 Tools & Technologies
- [LangGraph ReAct Agents](https://python.langchain.com/docs/langgraph)
- [FastAPI](https://fastapi.tiangolo.com/) for backend
- [Streamlit](https://streamlit.io/) for frontend
- [Groq](https://groq.com/) & [OpenAI](https://platform.openai.com/) LLM APIs  
- [Tavily Search API](https://tavily.com/) for real-time search
- [LangChain](https://www.langchain.com/) for tools
- [Uvicorn](https://www.uvicorn.org/) ASGI server
- Python 3.10+
- VS Code for development

---

## 📌 Architecture
[User Query]
|
[Streamlit UI] ---> [FastAPI Backend] ---> [AI Agent]
↳ LLM (Groq/OpenAI)
↳ Tavily (Search Tool)
|
[Response to UI]


---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository
git clone https://github.com/prathmkapde17/AI-Agent-Chatbot-with-FastAPI-and-LangGraph.git
cd AI-Agent-Chatbot-with-FastAPI-and-LangGraph



### 2️⃣ Create Virtual Environment
python -m venv venv
source venv/bin/activate # Mac/Linux
venv\Scripts\activate # Windows



### 3️⃣ Install Dependencies
pip install -r requirements.txt


_or if using Pipenv_:
pipenv install



### 4️⃣ Setup Environment Variables
Create a `.env` file in the root and add:
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key



---

## ▶️ Running the Application

### Run Backend Server (FastAPI)
uvicorn backend:app --reload --host 0.0.0.0 --port 8000


Test API at:  
📄 Swagger UI → `http://localhost:8000/docs`  
📄 Redoc UI → `http://localhost:8000/redoc`

### Run Frontend (Streamlit)
streamlit run frontend.py


UI will be live at:  
🌐 `http://localhost:8501`

---

## 📜 File Structure
AI-Agent-Chatbot-with-FastAPI-and-LangGraph/
│── ai_agent.py # Core AI Agent (LangGraph & tools)
│── backend.py # FastAPI server
│── frontend.py # Streamlit UI
│── requirements.txt # Python dependencies
│── Pipfile / .lock # If using Pipenv
│── .env # API Keys (not in repo)
│── README.md # Project documentation
│── AI Chatbot–GenAI Application (Production Ready).pdf



---

## 📹 Usage Flow
1. Select **model provider** (Groq, OpenAI, etc.)
2. Select **model name** (Llama, Mistral, GPT-4, etc.)
3. Set **system prompt** for personality/context
4. Enter **user query**
5. Get AI-driven answer with optional live search integration

---

## 📌 Future Improvements
- Add **multi-turn memory**
- Enable **RAG with local PDFs**
- Deploy to cloud platforms (Render, Hugging Face Spaces, AWS)
- Add **authentication for API**

---

## 📄 License
MIT License – free to use and modify.

---

## 🙌 Acknowledgements
- [LangChain](https://www.langchain.com/) & [LangGraph](https://python.langchain.com/docs/langgraph) for agent framework
- [Tavily](https://tavily.com/) for real-time search
- [FastAPI](https://fastapi.tiangolo.com/) & [Streamlit](https://streamlit.io/) for web development
- [Groq](https://groq.com/) & [OpenAI](https://platform.openai.com/) for LLM APIs
