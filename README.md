# 🤖 Chat with Your Data – AI-Powered File-Aware Chatbot

This project is an interactive chatbot that lets users **talk directly with their data**. Think of it as ChatGPT, but trained on your custom file — like a 1000-page book, an Excel sheet, or any structured dataset.

With this app, you can upload a file (e.g., an Excel spreadsheet), and instantly chat with an intelligent agent that can interpret the data, provide answers, and engage in natural conversation — all powered locally using [Ollama](https://ollama.ai) and the `gemma3` model.

---

## 🚀 Features

- 🧠 **Custom Data Chatbot**: Upload any Excel file and interact with it as if you're chatting with an expert who read the whole thing.
- 🔧 **Powered by Ollama LLM**: Uses the lightweight and fast `gemma3` model running locally.
- 📈 **Excel File Support**: Load `.xlsx` and `.xls` files with full context awareness.
- 💬 **Conversational Interface**: Built with [Gradio](https://gradio.app) for a beautiful, interactive chat UI.
- 🦾 **LangChain Integration**: Utilizes LangChain's `pandas` agent for dataframe-based question answering.
- 🗃️ **Extensible Framework**: Can be adapted to work with books, PDFs, or other file types with minor modifications.

---

## 📸 Demo

<!-- Add a screenshot if you have one -->
![Chatbot demo pic](https://github.com/user-attachments/assets/f9e41b51-785b-4dcf-af0f-5c2b033fed90)


---

## 🧑‍💻 How It Works

1. **Upload** an Excel file.
2. The backend loads the file into a `pandas.DataFrame`.
3. A LangChain agent is initialized using the `gemma3` model from Ollama.
4. Ask natural-language questions about your data — and get accurate, concise answers.

### Example Prompts

- “What is the total revenue for Q2?”
- “List all customers from New York.”
- “What are the top 5 products by sales?”
- “Hi!” → Get a friendly greeting from the chatbot 🤖

---

## 📂 Tech Stack

- **Python**
- **Ollama + Gemma3** (local LLM inference)
- **LangChain**
- **Gradio**
- **pandas / openpyxl**

---

## ⚙️ Setup Instructions

### Requirements

- Python 3.9+
- Ollama installed locally with `gemma3` pulled:  
  ```bash
  ollama pull gemma3
