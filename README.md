# Hi, I'm Qianmu 👋

I'm a **Software Engineering M.S. student at South China Normal University (Class of 2028)**.

I focus on **LLM application development, Multi-Agent systems, and Java backend engineering**, with an interest in building reliable, practical, and evidence-grounded AI applications.

My projects cover multi-agent research workflows, enterprise RAG and tool-calling applications, asynchronous AI task processing, and MCP tool security. I also conduct research on multimodal visual question answering, document understanding, and parameter-efficient fine-tuning.

## 🚀 Featured Projects

### 1. [ResearchPilot: Multi-Agent Research & Report Generation Platform](https://github.com/qianmu233/research-pilot)

**ResearchPilot：多智能体自主调研与报告生成平台**

`Python` `FastAPI` `LangChain` `LangGraph` `Multi-Agent` `RAG` `Pydantic` `BGE` `PgVector` `SQLite`

- Developed a **Supervisor-Worker multi-agent architecture** for enterprise technology evaluation and multi-document research, supporting both single-agent and multi-agent execution modes.
- Implemented dynamic task decomposition, parallel research through LangGraph subgraphs and Send, independent worker states, global evidence assessment, and targeted supplemental retrieval.
- Integrated Chinese semantic retrieval, evidence deduplication, source ID validation, and excerpt verification. Implemented atomic model-call budget management with SQLite and subtask-level crash recovery with persistent execution states and LangGraph Checkpointer.
- On a retrieval benchmark containing 19 test documents and 16 answerable questions, improved **Recall@5 from 53.125% to 100%** and **MRR@5 from 51.04% to 96.875%** by switching from English BGE to Chinese BGE.
- Across 18 controlled Mock runs on two synthetic enterprise research tasks, improved key-evidence coverage from **12/21 with a single agent to 21/21 with dynamic multi-agent orchestration**. Passed 124 automated regression tests and validated subtask-level recovery after process crashes.

### 2. [Enterprise Knowledge Base & ERP Q&A Platform](https://github.com/qianmu233/enterprise-rag-erp-assistant)

**企业知识库与 ERP 智能问答平台**

`Java 17` `Spring Boot` `Spring AI` `ChatClient` `RAG` `Function Calling` `PgVector` `SSE`

- Extended an existing Spring AI application combining **RAG and agent-style tool calling** for enterprise knowledge retrieval, ERP data queries, and hybrid question answering.
- Improved SSE streaming response processing through cross-chunk buffering and incremental sanitization, preserving ERP business fields while filtering internal model markers and tool-execution messages.
- Added tool-calling protocol tests covering streamed arguments, tool-result responses, token usage, and SSE completion events. Conducted response diagnostics and six offline retrieval comparison experiments.
- Across three evaluation rounds on a fixed 50-question dataset, reduced empty answers from **25/50 to 0/50** and improved literal key-fact phrase matching from **36.73% to 53.06%**.

Based on [ly1836/spring-ai-rag-demo](https://github.com/ly1836/spring-ai-rag-demo), with project modifications and upstream implementation boundaries documented in the repository.

### 3. [Asynchronous AI Task Processing Platform](https://github.com/qianmu233/async-ai-task-platform)

**大模型异步任务处理平台**

`Java 17` `Spring Boot` `MySQL` `RabbitMQ` `Redis` `Lua` `Transactional Outbox`

- Built an asynchronous task processing platform for long-running LLM requests, decoupling task acceptance, background execution, and result retrieval.
- Implemented idempotent submission, persistent task states, Transactional Outbox, RabbitMQ publisher confirms and returns, conditional worker claims, execution-token validation, timeout protection, and Redis Lua rate limiting.
- Integrated Mock and OpenAI-compatible model providers with bounded HTTP response sizes and controlled error handling.
- In a local benchmark using a fixed 1,000 ms Mock model delay, eight concurrent requests, and 240 requests per mode, reduced p95 response time from **1,019.125 ms for synchronous requests to 2.245 ms for asynchronous task acceptance**.
- In a standalone JAR verification, successfully dispatched all 25 Outbox events; 24 normal tasks succeeded, and one simulated model failure reached its expected failed state.

### 4. [Agent Tool Invocation Security Gateway](https://github.com/qianmu233/agent-security-gateway)

**Agent 工具调用安全授权网关**

`Java 17` `Spring Security` `MCP` `LangGraph` `API Key` `RBAC`

- Built an MCP tool security gateway integrating a Python LangGraph Agent with a Java backend, enforcing server-side identity mapping, RBAC, tenant-based access control, resource authorization, and audit logging.
- Implemented a one-time **Write Intent** mechanism with a 60-second expiration, binding authorization to the user, tool, tenant, order, and modification quantity. Used synchronized authorization consumption to prevent concurrent replay within a single JVM.
- Validated **24 MCP HTTP security scenarios**, with 8/8 authorized requests accepted and 16/16 unauthorized requests rejected. Additional concurrency tests covered 280 requests, including 220 rejected replay attempts.

## 🛠️ Tech Stack

- **Languages:** Java · Python · SQL · C++
- **LLM Application Development:** Spring AI · LangChain · ChatClient · Function Calling · SSE · MCP
- **Multi-Agent & Workflow:** LangGraph · Supervisor-Worker · Parallel Subgraphs · Conditional Routing · Checkpointing · Pydantic
- **RAG & Retrieval:** BGE · Embedding · PostgreSQL · PgVector · ONNX Runtime · Recall@K · MRR@K
- **Backend Engineering:** Spring Boot · Spring Security · FastAPI · MySQL · RabbitMQ · Redis · SQLite · REST API
- **Testing & Infrastructure:** JUnit 5 · pytest · Docker · Docker Compose · Maven · Git · Linux
- **AI Research:** PyTorch · Multimodal Learning · Visual Question Answering · LoRA

## 🔬 Research Interests

- OCR-Rich Visual Question Answering
- Multimodal Document Understanding
- Parameter-Efficient Fine-Tuning
- Evidence-Grounded LLM Applications

First author of two research papers, with one accepted and one under review.

## 🎯 Career Interests

Open to internship opportunities in:

- LLM Application Development
- AI Agent & Multi-Agent Development
- Java Backend Engineering
- AI Platform Engineering

**Availability:** 5+ days per week · 6+ months · Available immediately

Thanks for visiting my profile! 👋
