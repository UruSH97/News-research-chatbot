# NewsBot – AI-Powered News Research Tool

**NewsBot** is an AI-powered research assistant that allows users to input up to 3 news article URLs and ask questions based on the content from those articles. The system fetches, splits, embeds, and indexes article content using OpenAI and LangChain, enabling real-time Q&A with accurate source attribution.

---

## Problem Statement
In an age of information overload, keeping up with news while maintaining fact accuracy is challenging. This project aims to simplify that by building an intelligent assistant that extracts news from provided URLs and allows users to interact with the content meaningfully through question-answering.

---

## Features

- Accepts multiple news article URLs (via sidebar)
- Scrapes and parses the full article content
- Splits text intelligently using `RecursiveCharacterTextSplitter`
- Converts text into embeddings using `OpenAIEmbeddings`
- Stores embeddings in `FAISS` for fast semantic search
- Enables question-answering over the articles with source citations using LangChain's `RetrievalQAWithSourcesChain`
- Built with an interactive Streamlit UI

---

## Tech Stack

- Python
- Streamlit
- OpenAI API
- LangChain
- FAISS
- dotenv
- Pickle

---

##  How to Run

```bash
# 1. Clone the repo
git clone https://github.com/your-username/newsbot-langchain-research

# 2. Navigate to the directory
cd newsbot-langchain-research

# 3. Install dependencies
pip install -r requirements.txt

# 4. Add your OpenAI API key in a `.env` file
OPENAI_API_KEY=your_openai_key

# 5. Run the app
streamlit run app.py

---
![NewsBot](NewsBot.jpg)
