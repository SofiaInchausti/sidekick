# Sidekick AI: Your Personal Work Companion

**Sidekick AI** is an intelligent agentic assistant built with **LangGraph**, **LangChain**, and **Gradio**. It leverages a multi-node graph architecture to perform tasks, browse the web using **Playwright**, execute Python code, and self-evaluate its own performance against user-defined success criteria.



## 🚀 Features

* **Autonomous Agent**: Uses a ReAct-style worker to use tools and solve complex queries.
* **Self-Evaluation Loop**: Includes an "Evaluator" node that checks if the output meets the user's specific success criteria before finishing.
* **Web Automation**: Integrated with Playwright for real-time web browsing and information retrieval.
* **Toolbox**: Includes Google Search (Serper), Wikipedia, Python REPL, and File Management.
* **Persistent Memory**: Uses `MemorySaver` to maintain conversation context across steps.
* **Modern UI**: Built with Gradio 6.0 for a clean, responsive chat experience.

---

## 🛠️ Tech Stack

* **Core Logic**: [Python 3.12+](https://www.python.org/)
* **Orchestration**: [LangGraph](https://github.com/langchain-ai/langgraph)
* **LLM**: OpenAI (GPT-4o-mini)
* **UI Framework**: [Gradio 6.0](https://gradio.app/)
* **Automation**: [Playwright](https://playwright.dev/python/)

---

## 📦 Installation & Setup

### 1. Clone the repository
```bash
git clone [https://github.com/yourusername/sidekick-ai.git](https://github.com/yourusername/sidekick-ai.git)
cd sidekick-ai
```
### 2. **Configure the virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

### 3. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

### 4. **Configure Environment Variables:**
    Create a `.env` file in the root directory and add your credentials:
    ```env
    OPENAI_API_KEY=your_openai_key
    PUSHOVER_TOKEN=pushover_token
    PUSHOVER_USER=pushover_user
    HF_TOKEN=hf_token
    LANGSMITH_TRACING=langsmith_tracing
    LANGSMITH_ENDPOINT=langsmith_endpoint
    LANGSMITH_API_KEY=lagsmith_api_key
    LANGSMITH_PROJECT=langsmith_project
    SERPER_API_KEY=serper_api_key
    ```

### 5. **Run the application:**
    ```bash
    python app.py
    ```# Sidekick