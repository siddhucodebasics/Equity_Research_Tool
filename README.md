# 📊 Equity Research Tool — Multi-Source LLM-Powered RAG System

## 🚀 Project Overview
The **Equity Research Tool** is an **LLM-powered Retrieval-Augmented Generation (RAG) system** designed to support equity research analysts by aggregating and reasoning over **multiple online research sources**.

Unlike static PDF-based tools, this system works with **live research links** such as:
- Financial news articles
- Company analysis blogs
- Market commentary
- Public research reports

The tool retrieves relevant information from multiple sources and generates **context-aware, grounded answers**, closely simulating real-world equity research workflows.

---

## 🧠 Key Features
- 🔗 Accepts **multiple research URLs** as input  
- 🧹 Cleans and normalizes web-based textual content  
- ✂️ Splits text into semantic chunks for better retrieval  
- 🔎 Performs semantic search using **FAISS vector database**  
- 🤖 Uses OpenAI embeddings for high-quality retrieval  
- 💬 Generates context-aware answers using an LLM (RAG)  
- 🔐 Secure API key handling via environment variables  

---

## 🏗️ High-Level Architecture

Research URLs (Multiple Sources)
↓
Web Content Loader
↓
Text Cleaning & Chunking
↓
OpenAI Embeddings
↓
FAISS Vector Store
↓
Retriever
↓
LLM Answer Generation

---

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **LLM Framework:** LangChain  
- **Vector Database:** FAISS  
- **Embeddings:** OpenAI Embeddings  
- **Data Ingestion:** Web-based content loaders  
- **Environment:** Jupyter Notebook  

---

## 📁 Project Structure
Equity_Research_Tool/
├── Equity_research_tool_code.ipynb # End-to-end RAG pipeline
├── Requirements.txt # Python dependencies
├── .gitignore # Security & clean repository

> ⚠️ FAISS index files are intentionally excluded from GitHub and generated locally.

---

## ⚙️ How the Tool Works
1. Analysts provide **multiple research URLs**
2. Content is fetched and cleaned
3. Text is split into meaningful chunks
4. Embeddings are generated and stored in FAISS
5. Relevant chunks are retrieved for each query
6. The LLM generates **context-grounded insights**

---

## ⚙️ How to Run the Project

1️⃣ Clone the Repository
git clone https://github.com/siddhucodebasics/Equity_Research_Tool.git
cd Equity_Research_Tool

2️⃣ Install Dependencies
pip install -r Requirements.txt

3️⃣ Set OpenAI API Key
Windows (PowerShell):
setx OPENAI_API_KEY "your_api_key_here"

4️⃣ Run the Notebook
Open and execute:
Equity_research_tool_code.ipynb

🧪 Example Questions

“Summarize bullish vs bearish views across sources”

“What risks are repeatedly mentioned?”

“Compare growth outlook from different analysts”

“Highlight contradictions between sources”

🔒 Security & Best Practices

✅ API keys stored using environment variables

✅ No secrets committed to GitHub

✅ Vector index excluded using .gitignore
