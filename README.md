# Hi, I'm Qianmu 👋

I'm a **Software Engineering M.S. student at South China Normal University (Class of 2028)**.

I focus on **Java backend engineering, LLM application development, and Agent systems**, with an interest in building reliable, practical, and secure AI-powered applications.

My projects cover asynchronous AI task processing, LangGraph research agents, enterprise RAG applications, and MCP tool security. I also conduct research on multimodal visual question answering and parameter-efficient fine-tuning.

## 🚀 Featured Projects

### 1. [Asynchronous AI Task Orchestration Platform](https://github.com/qianmu233/async-ai-task-platform)

**大模型异步任务处理平台**

`Java 17` `Spring Boot` `MySQL` `RabbitMQ` `Redis` `Lua`

- Built an asynchronous task processing system supporting idempotent submission, persistent task states, background execution, and result retrieval.
- Implemented **Transactional Outbox**, RabbitMQ Publisher Confirm/Return, conditional worker claims, and execution-token-based timeout protection. Integrated Mock and OpenAI-compatible model providers with Redis Lua rate limiting.
- In a local benchmark using a 1,000 ms Mock model and 8 concurrent requests, reduced p95 API response time from **1,019.125 ms for synchronous requests to 2.245 ms for asynchronous task acceptance**.

### 2. [ResearchPilot: Multi-Document Research & Report Generation Agent](https://github.com/qianmu233/research-pilot)

**ResearchPilot：多文档自主调研与报告生成 Agent**

`Python` `FastAPI` `LangGraph` `RAG` `PgVector` `SQLite`

- Developed a five-node **LangGraph workflow** for research planning, retrieval, evidence assessment, report generation, and citation validation, with conditional routing for supplemental retrieval.
- Implemented Chinese semantic retrieval using BGE-small-zh-v1.5, source ID validation, and excerpt verification for structured reports. Integrated SQLite task persistence, LangGraph Checkpointer, and persistent model-call budgets for task recovery.
- On an evaluation set of 19 synthetic documents and 16 answerable questions, improved **Recall@5 from 53.125% to 100%** and **MRR@5 from 51.04% to 96.875%**.

### 3. [Enterprise Knowledge Base & ERP Q&A Platform](https://github.com/qianmu233/enterprise-rag-erp-assistant)

**企业知识库与 ERP 智能问答平台**

`Java 17` `Spring AI` `RAG` `PgVector` `ONNX Runtime` `SSE`

- Contributed to an existing Spring AI application integrating enterprise knowledge retrieval and ERP tool calling, with a focus on streaming response handling, model integration testing, and retrieval evaluation.
- Improved **SSE streaming processing** through cross-chunk buffering and incremental sanitization, preserving ERP business fields while filtering internal model markers. Added tool-calling protocol tests, response diagnostics, and offline retrieval experiments.
- Across three evaluation rounds on a 50-question dataset, reduced empty answers from **25/50 to 0/50** and improved literal key-fact phrase matching from **36.73% to 53.06%**.

Based on [ly1836/spring-ai-rag-demo](https://github.com/ly1836/spring-ai-rag-demo), with project modifications and source boundaries documented in the repository.

### 4. [Agent Tool Invocation Security Gateway](https://github.com/qianmu233/agent-security-gateway)

**Agent 工具调用安全授权网关**

`Java 17` `Spring Security` `MCP` `LangGraph` `API Key` `RBAC`

- Built an MCP tool security gateway integrating a Python LangGraph Agent with a Java backend, enforcing server-side identity mapping, RBAC, tenant isolation, resource authorization, and audit logging.
- Implemented a one-time **Write Intent** mechanism with a 60-second expiration, binding authorization to the user, tool, tenant, order, and modification quantity. Used synchronized authorization consumption to prevent concurrent replay within a single JVM.
- Validated **24 MCP HTTP security scenarios**, with 8/8 authorized requests accepted and 16/16 unauthorized requests rejected. Additional concurrency tests covered **280 requests, including 220 rejected replay attempts**.

## 🛠️ Tech Stack

- **Languages:** Java · Python · SQL · C++
- **Backend Development:** Spring Boot · Spring Security · MySQL · RabbitMQ · Redis · REST API
- **LLM & Agent Development:** Spring AI · LangChain · LangGraph · RAG · MCP · FastAPI
- **Retrieval & Data:** PostgreSQL · PgVector · BGE · ONNX Runtime · SQLite
- **Testing & Infrastructure:** JUnit 5 · pytest · Docker · Docker Compose · Maven · Git

## 🎯 Career Interests

Open to internship opportunities in:

- Java Backend Engineering
- LLM Application & Agent Development
- AI Platform Engineering

Thanks for visiting my profile! 👋
