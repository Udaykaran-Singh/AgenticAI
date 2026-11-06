# Agentic AI 🤖

A hands-on collection of implementations, experiments, and learning resources focused on **Agentic AI, Large Language Models (LLMs), and AI application development**.

This repository documents my journey of exploring the modern AI ecosystem, with practical implementations using LangChain, LangGraph, and LangSmith.

The goal is to understand how LLM-powered applications work, build intelligent workflows, implement Retrieval-Augmented Generation (RAG), and develop autonomous AI agents.

## 📚 Technologies & Frameworks

- **Python** – Primary programming language
- **LangChain** – Framework for building LLM-powered applications
- **LangGraph** – Stateful, multi-step AI workflows and agent orchestration
- **LangSmith** – Debugging, tracing, monitoring, and evaluating LLM applications
- **OpenAI** – Large Language Models and embeddings
- **Anthropic** – Claude models
- **Google AI** – Gemini models
- **Hugging Face** – Open-source models and embeddings

## 📂 Repository Structure

```text
AgenticAI/
│
├── LangChain/
│   ├── 1_Models/
│   │   ├── 1_LLMs/
│   │   ├── 2_Chat_Models/
│   │   └── 3_Embedding_Models/
│   │
│   ├── 2_Prompts/
│   ├── 3_Structured_Outputs/
│   ├── 4_Output_parser/
│   ├── 5_Chains/
│   ├── 6_Runnables/
│   │
│   ├── 7_RAG/
│   │   ├── 1_Document_Loader/
│   │   ├── 2_Text_splitters/
│   │   ├── 3_vector_store.py
│   │   └── RAG.py
│   │
│   └── 8_Agents/
│
├── LangGraph/
│   ├── 01_bmi_workflow.ipynb
│   ├── 02_simple_llm_workflow.ipynb
│   ├── 03_prompt_chaining.ipynb
│   ├── 04_Simple_Parallel_batsman_workflow.ipynb
│   ├── 05_Parallel_llm_UPSC_essay_workflow.ipynb
│   ├── 06_Conditional_Workflow_quadratic_equation_workflow.ipynb
│   ├── 07_Conditional_Workflow_llm_review_reply_workflow.ipynb
│   ├── 08_Loop_X_post_generator.ipynb
│   ├── 09_basic_chatbot.ipynb
│   ├── 10_persistence.ipynb
│   ├── 11_tools.ipynb
│   ├── 12_mcp.py
│   ├── 13_rag.ipynb
│   ├── 14_HITL.ipynb
│   ├── 15_1_subgraphs.ipynb
│   ├── 15_2_subgraph_shared.ipynb
│   │
│   ├── chatbot-in-langgraph-main/
│   └── memory-in-llms-main/
│
├── LangSmith/
│   ├── 1_simple_llm_call.py
│   ├── 2_sequential_chain.py
│   ├── 3_rag_v1.py
│   ├── 3_rag_v2.py
│   ├── 3_rag_v3.py
│   ├── 3_rag_v4.py
│   ├── 4_agent.py
│   └── 5_langgraph.py
│
├── requirements.txt
└── .gitignore
```

## 🧠 Topics Covered

### 1. LangChain

Exploring the core components of LangChain for developing LLM-powered applications.

| Topic | Concepts |
|---|---|
| Models | LLMs, Chat Models, Embedding Models |
| Prompts | Prompt Templates, Chat Prompts, Message Placeholders |
| Structured Outputs | TypedDict, Pydantic, JSON Schema |
| Output Parsers | String, JSON, Pydantic, Structured Output |
| Chains | Simple, Sequential, Parallel, Conditional Chains |
| Runnables | Sequence, Parallel, Branch, Lambda, Passthrough |
| RAG | Document Loaders, Text Splitters, Vector Stores, Retrieval |
| Agents | Tools, Tool Calling, Agent Execution |

### 2. LangGraph

Learning to build stateful and controllable AI workflows using graph-based orchestration.

**Topics and implementations:**

- Basic LLM workflows
- Prompt Chaining
- Parallel Workflows
- Conditional Workflows
- Loop-based Workflows
- AI Chatbots
- Persistence and Memory
- Tool Integration
- Model Context Protocol (MCP)
- Retrieval-Augmented Generation (RAG)
- Human-in-the-Loop (HITL)
- Subgraphs and Shared State
- Short-Term Memory (STM)
- Long-Term Memory (LTM)
- Database-backed Memory

**Additional Implementations:**

- Chatbot with and without Human-in-the-Loop
- LangGraph Chatbot with Tool Calling
- RAG-based Chatbot
- Database-integrated Chatbot
- MCP-integrated Chatbot
- Streaming and Threading
- Memory Management

### 3. LangSmith

Exploring observability, debugging, and monitoring for LLM applications.

**Topics covered:**

- LLM Tracing
- Sequential Chain Monitoring
- RAG Application Tracing
- Agent Execution Tracking
- LangGraph Tracing
- Debugging and Observability

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Udaykaran-Singh/AgenticAI.git
```

### 2. Navigate to the Project

```bash
cd AgenticAI
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it:

**macOS / Linux**

```bash
source .venv/bin/activate
```

**Windows**

```bash
.venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure API Keys

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
GOOGLE_API_KEY=your_google_api_key
LANGCHAIN_API_KEY=your_langsmith_api_key
LANGCHAIN_TRACING_V2=true
LANGCHAIN_PROJECT=AgenticAI
```

Never commit your `.env` file or expose API keys publicly.

### 6. Run Examples

For LangChain:

```bash
python LangChain/1_Models/1_LLMs/llm_demo.py
```

For LangGraph:

Open the notebooks inside the `LangGraph/` directory using Jupyter Notebook or VS Code.

For LangSmith:

```bash
python LangSmith/1_simple_llm_call.py
```

## 🎯 Learning Objectives

- Understand the architecture and capabilities of Large Language Models.
- Build LLM-powered applications using LangChain.
- Implement prompt engineering and structured output generation.
- Develop RAG pipelines using document loaders, text splitters, and vector stores.
- Build intelligent agents with tool-calling capabilities.
- Design stateful and multi-agent workflows using LangGraph.
- Implement short-term and long-term memory.
- Explore Human-in-the-Loop interactions and MCP.
- Monitor, debug, and evaluate AI applications using LangSmith.

## 📈 Progress

This repository is an ongoing collection of my Agentic AI learning journey. It will continue to evolve with new experiments, implementations, and projects as I explore the rapidly growing ecosystem of AI agents and LLM applications.

---

**Exploring the future of AI, one agent at a time.** 🚀
