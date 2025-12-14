# LangGraph Chatbot with Groq (Simple Chatbox)

A minimal, clean example of building a conversational chatbot using **LangGraph** and **Groq's** fast inference API.

This notebook demonstrates:
- Setting up a stateful conversation graph with LangGraph
- Using `ChatGroq` to call a large open-source model (`openai/gpt-oss-120b`)
- Two interaction modes:
  - Synchronous streaming (full response at once)
  - Async token-by-token streaming (real-time typing effect)

Perfect for learning LangGraph basics or as a starting template.

## Features

- No LangSmith tracing warnings (disabled by default)
- Clean message handling for both old and new LangGraph versions
- Real-time token streaming using `astream_events` + `nest_asyncio`
- Simple quit command (`q` or `quit`)
- Graph visualization (Mermaid diagram)

## Requirements

- Python 3.9+
- Google Colab (or Jupyter notebook) recommended for easy setup
- Packages installed via:
  ```bash
  pip install langgraph langchain langchain_groq langchain_community nest_asyncio




  Setup (Google Colab)Open this notebook in Google Colab

-Open this notebook in Google Colab

-Go to Runtime → Change runtime type → Hardware accelerator → GPU (optional, for faster inference)

-In Colab secrets (left sidebar → ), add two secrets:Groq_Api_Key → your Groq API key (get it free at https://console.groq.com/keys)

-langsmith_api_key → your LangSmith key (optional, can be empty since tracing is disabled)

-Run all cells
