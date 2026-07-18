# GenAI: LangChain Introduction & Model Integration

Welcome to **GenAI**, a hands-on workspace demonstrating how to build LLM-powered applications using **LangChain**, **Google Gemini**, and **Groq**. 

This repository contains step-by-step guides and Jupyter notebooks illustrating model integration, environment configuration, and clean invocations across multiple LLM providers.

---

## 🚀 Features

- **LangChain Version V1 Compatibility:** Uses standard modern LangChain orchestration techniques.
- **Google Gemini Integration:** Integrates `gemini-3.5-flash` natively using the consolidated `langchain-google-genai` interface.
- **Groq Integration:** Invokes fast inference models like `llama-3.1-8b-instant` and `qwen/qwen3.6-27b` using the `langchain-groq` library.
- **Unified Model Init:** Demonstrates the use of LangChain's consolidated `init_chat_model` API to seamlessly switch between model backends.

---

## 📂 Project Structure

- `generativeai/1-langchainintro.ipynb` - Core Jupyter notebook containing the LangChain introductory tutorial.
- `requirements.txt` - Python project dependencies.
- `pyproject.toml` & `uv.lock` - Modern python project management configuration powered by **uv**.

---

## 🛠️ Getting Started

### Prerequisites

- [Python 3.10+](https://www.python.org/downloads/)
- [uv](https://github.com/astral-sh/uv) (recommended fast package manager) or standard `pip`

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/akshitbansal2005/GenAI.git
   cd GenAI
   ```

2. **Set up the Virtual Environment & Dependencies:**
   If using `uv` (recommended):
   ```bash
   uv venv
   uv pip install -r requirements.txt
   ```
   If using standard `pip`:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows, use: .venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root of the project directory and add your API keys:
   ```env
   GROQ_API_KEY="your-groq-api-key-here"
   GEMINI_API_KEY="your-gemini-api-key-here"
   ```

---

## 📓 Running the Notebook

To run the interactive tutorials in your notebook environment:

1. Register the virtual environment kernel:
   ```bash
   python -m ipykernel install --user --name=GenAI --display-name "Python (GenAI)"
   ```
2. Open the notebook in VS Code or run Jupyter Lab:
   ```bash
   jupyter lab
   ```
3. Open `generativeai/1-langchainintro.ipynb` and run the cells!