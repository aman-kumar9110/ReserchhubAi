🚀 ResearchHub AI – Intelligent Agentic RAG Platform

ResearchHub AI is a smart, full-stack system designed for managing and analyzing research papers. The platform enables users to upload complex academic documents, extract meaningful insights, and interact with a context-aware AI assistant. The assistant maintains conversation memory and is designed to minimize hallucinations by responding only with information derived from the uploaded papers.

✨ Core Features
🧠 Context-Aware AI Memory

The assistant uses Llama-3.1 (through Groq) to maintain short-term conversational context. This allows users to ask follow-up questions naturally without repeating previous information.

📚 Multi-Paper Analysis

Users can upload and select multiple research papers and query them together. The AI can analyze, compare, and synthesize insights from different documents simultaneously.

🚫 Hallucination Prevention

The system is designed with strict contextual boundaries. If a query is unrelated to the uploaded research papers, the AI will clearly state that it cannot answer, ensuring high reliability and factual responses.

📝 Integrated DocSpace Editor

A built-in rich text editor allows users to write research notes and summaries. All notes are synchronized with the backend database for easy access and management.

🗂️ Interactive Dashboard

The dashboard provides an overview of active workspaces, uploaded documents, and quick AI tools for document analysis.

💻 Technology Stack
Frontend

React.js with TypeScript

Tailwind CSS for responsive UI design

Lucide Icons

React-Quill for the rich text editing interface

Backend

FastAPI for high-performance API development

SQLAlchemy with SQLite for database management

PyMuPDF (fitz) for accurate PDF text extraction

AI & LLM Engine

Groq API as the inference engine

Llama-3.1-8B-Instant as the primary model for reasoning, summarization, and contextual responses

🚀 Installation & Setup

Follow these steps to run the project locally.

1️⃣ Backend Setup

Navigate to the backend directory and create a virtual environment.

cd backend
python -m venv venv

Activate the environment:

source venv/bin/activate   # Windows: venv\Scripts\activate

Install the required dependencies:

pip install -r requirements.txt

Create a .env file in the backend folder and add your Groq API key:

GROQ_API_KEY=your_api_key_here

Start the FastAPI server:

uvicorn main:app --reload
2️⃣ Frontend Setup

Open a new terminal and run the frontend application.

cd frontend
npm install
npm run dev
🛡️ Security & Privacy

Local Data Storage: Uploaded PDFs and extracted content are stored locally.

Protected Files: Sensitive files such as .env, node_modules, __pycache__, and database files are excluded using .gitignore.

Data Safety: API keys and confidential data are not pushed to the repository.

👨‍💻 Developed By

Adarsh Patel,Amit kumar,Abhishek Chauhan,Aman Kumar
