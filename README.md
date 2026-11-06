# Agentic AI

A structured collection of **Agentic AI concepts, practical implementations, and Python projects**, covering Large Language Models (LLMs), LLM-powered applications, Retrieval-Augmented Generation (RAG), AI agents, and stateful workflow orchestration.

This repository contains my learning journey through the modern AI ecosystem, with hands-on implementations, experiments, and practical examples using LangChain, LangGraph, LangSmith, and various LLM providers.

## Topics Covered

| No. | Topic | Concepts |
|---|---|---|
| 01 | LangChain – Models | Large Language Models (LLMs), Chat Models, Embedding Models |
| 02 | Prompt Engineering | Prompt Templates, Chat Prompts, Message Placeholders |
| 03 | Structured Outputs | TypedDict, Pydantic, JSON Schema, Structured Response Generation |
| 04 | Output Parsers | String Output Parser, JSON Output Parser, Pydantic Output Parser |
| 05 | Chains | Simple Chains, Sequential Chains, Parallel Chains, Conditional Chains |
| 06 | Runnables | Runnable Sequence, Runnable Parallel, Runnable Branch, Runnable Lambda, Runnable Passthrough |
| 07 | Retrieval-Augmented Generation (RAG) | Document Loaders, Text Splitters, Vector Stores, Embeddings, Retrieval Pipelines |
| 08 | AI Agents | Agent Architecture, Tool Calling, Tool Integration, Agent Execution |
| 09 | LangGraph – Workflows | Basic LLM Workflows, Prompt Chaining, Parallel Workflows, Conditional Workflows, Loop-based Workflows |
| 10 | LangGraph – Chatbots | Basic Chatbots, Stateful Chatbots, Conversational Workflows |
| 11 | Memory and Persistence | Short-Term Memory (STM), Long-Term Memory (LTM), Persistence, Database-backed Memory |
| 12 | Tool Integration and MCP | Tool Calling, Model Context Protocol (MCP), External Tool Integration |
| 13 | LangGraph – RAG | RAG-based Workflows, Retrieval Integration, Context-aware Chatbots |
| 14 | Human-in-the-Loop (HITL) | Human Approval, Interruptions, Human-in-the-Loop Workflows |
| 15 | Subgraphs | Subgraphs, Shared State, Modular Workflow Design |
| 16 | LangSmith | LLM Tracing, Debugging, Monitoring, Observability, Application Evaluation |

## Repository Structure

The repository is organized framework-wise, with separate directories for LangChain, LangGraph, and LangSmith implementations.

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

*Note: The directory names and numbering above follow the current local repository structure.*

## Tech Stack

- **Programming Language:** Python
- **Development Environment:** Jupyter Notebook, VS Code
- **LLM Framework:** LangChain
- **Workflow Orchestration:** LangGraph
- **LLM Observability:** LangSmith
- **LLM Providers:** OpenAI, Anthropic, Google AI
- **Open-Source Models:** Hugging Face
- **Data Validation:** Pydantic
- **Configuration Management:** Python-dotenv
- **APIs and Integrations:** Model APIs, Tools, MCP

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Udaykaran-Singh/AgenticAI.git
```

### 2. Navigate to the Project

```bash
cd AgenticAI
```

### 3. Create a Virtual Environment (Optional)

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

Create a `.env` file in the project root and add the required API credentials:

```env
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
GOOGLE_API_KEY=your_google_api_key

LANGCHAIN_API_KEY=your_langsmith_api_key
LANGCHAIN_TRACING_V2=true
LANGCHAIN_PROJECT=AgenticAI
```

*Note: Configure only the API keys required for the particular implementation. Never commit your `.env` file or expose API keys publicly.*

### 6. Run Examples

**For LangChain:**

```bash
python LangChain/1_Models/1_LLMs/llm_demo.py
```

**For LangGraph:**

Open the Jupyter notebooks inside the `LangGraph/` directory using Jupyter Notebook or VS Code.

```bash
jupyter notebook
```

**For LangSmith:**

```bash
python LangSmith/1_simple_llm_call.py
```

## Learning Resource

The concepts and practical implementations in this repository are based on my self-learning and practice, including the **CampusX Agentic AI learning resources**.

- [CampusX – YouTube Channel](https://www.youtube.com/@campusx-official)

## Purpose

The goal of this repository is to maintain an organized collection of my Agentic AI notes, practical implementations, experiments, and coding exercises while strengthening my understanding of LLM-powered applications, intelligent agents, RAG pipelines, workflow orchestration, and the development of autonomous AI systems.

## Author

**Udaykaran Singh**

B.Tech – Data Science  
National Institute of Technology, Jalandhar

- GitHub: [Udaykaran-Singh](https://github.com/Udaykaran-Singh)

---

⭐ If you find this repository useful, feel free to explore the implementations and learn along!
