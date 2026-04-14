# LLM Engineering: From Fundamentals to Production

This is a hands-on guide to mastering Large Language Models (LLMs). It uses a structured, code-first approach to learning how LLMs work. It also shows how to build production-grade AI systems, inspired by professional LLM engineering workflows.

## 🎯 Goal

To bridge the gap between AI theory and practical engineering. It does this by building tools, exploring model internals, and deploying functional AI applications.

## 📂 Repository Structure

The project is organized into five core modules:

### 1. Local LLM, API & Tokenization

*   **Local Inference:** Running models on your own hardware using Ollama or LM Studio.
*   **Cloud APIs:** Integrating with industry leaders like OpenAI, Anthropic, and Google Gemini.
*   **Tokenization:** Deep dive into BPE, SentencePiece, and understanding how token limits impact costs and performance.

### 2. Gradio

*   **UI Prototyping:** Building web interfaces for LLMs in minutes.
*   **Chat Interfaces:** Creating persistent chat histories and real-time streaming responses.
*   **Interactive Demos:** Building tools for document uploads and model parameter tuning.

### 3. RAG (Retrieval-Augmented Generation)

*   **Vector Databases:** Indexing and searching data with ChromaDB, Pinecone, or FAISS.
*   **Embeddings:** Comparing different embedding models (OpenAI vs. HuggingFace).
*   **Knowledge Retrieval:** Implementing semantic search, re-ranking, and context window management.

### 4. Fine-Tuning the Model

*   **Dataset Prep:** Curating, cleaning, and formatting JSONL data for training.
*   **PEFT & LoRA:** Using Parameter-Efficient Fine-Tuning to train models without massive compute.
*   **Evaluation:** Comparing base models against fine-tuned checkpoints to measure improvement.

### 5. Agents

*   **Function Calling:** Teaching LLMs to use external tools, calculators, and APIs.
*   **Autonomous Loops:** Building ReAct agents that can "think" and "act" sequentially.
*   **Multi-Agent Systems:** Coordinating specialized agents to solve complex, multi-step tasks.

## 🚀 Getting Started

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/talhamucar/llm_learning
    cd llm_learning
    ```

2.  **Install uv** (if not already installed):

    ```bash
    pip install uv
    ```

3.  **Set up your environment and install dependencies:**

    ```bash
    uv sync
    ```

    This creates a `.venv/` virtual environment and installs all dependencies from `pyproject.toml`.

4.  **Activate the environment** (optional — `uv run` handles this automatically):

    ```bash
    source .venv/bin/activate  # On Windows: .venv\Scripts\activate
    ```

5.  **Configure your API Keys:**

    Copy `.env.example` to `.env` and fill in your credentials:

    ```bash
    cp .env.example .env
    ```

    ```env
    OPENAI_API_KEY=your_openai_key
    ANTHROPIC_API_KEY=your_anthropic_key
    GOOGLE_API_KEY=your_google_gemini_key
    TAVILY_API_KEY=your_search_api_key  # Useful for Agents
    ```

6.  **Launch Jupyter:**

    ```bash
    uv run jupyter notebook
    ```
