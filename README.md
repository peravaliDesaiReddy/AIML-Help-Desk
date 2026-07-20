🤖 GenAI Academic Helpdesk
An AI-powered academic helpdesk system built using Flask, LangChain, ChromaDB, and HuggingFace.

The system uses Retrieval Augmented Generation (RAG) to answer questions from multiple PDF documents such as:

syllabus
placement information
hostel rules
college circulars
Features
Multi-PDF Question Answering
Semantic Search using Embeddings
Chroma Vector Database
RAG Architecture
Modern Chatbot UI
Real-time AI Responses

Technologies Used
Python
Flask
LangChain
ChromaDB
HuggingFace
Sentence Transformers
HTML
CSS
JavaScript
Project Structure
student-ai-helpdesk/
│
├── app.py
├── requirements.txt
├── uploads/
│   ├── syllabus.pdf
│   ├── placement.pdf
│   ├── hostel.pdf
│   └── circular.pdf
│
├── templates/
│   └── index.html
│
├── static/
│   └── style.css
Installation
1. Clone Repository
git clone https://github.com/jisha-max/student-ai-helpdesk.git
2. Install Dependencies
pip install -r requirements.txt
3. Run Application
python app.py
Open in Browser
http://127.0.0.1:5000
Architecture
Multiple PDFs
        ↓
PyPDFLoader
        ↓
Text Chunking
        ↓
Embeddings
        ↓
Chroma Vector DB
        ↓
Retriever
        ↓
LLM
        ↓
Generated Answer
Example Questions
What is placement eligibility?
What are hostel rules?
When do exams start?
What is library timing?
How It Works
PDFs are loaded using PyPDFLoader
Documents are split into chunks
Embeddings are created using sentence transformers
ChromaDB stores vectors
RetrievalQA fetches relevant chunks
FLAN-T5 generates answers
Future Improvements
Voice Assistant
Dynamic PDF Upload
Multi-language Support
Cloud Deployment
Developed By
name: P.Desai Reddy
