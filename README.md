# Hi, I'm Qianmu 👋

I'm a **Software Engineering M.S. student at South China Normal University**.

I focus on **Java backend engineering and LLM application development**, with an interest in building reliable, practical, and secure AI-powered systems.

My work spans asynchronous AI task processing, enterprise RAG applications, MCP tool security, and evidence-grounded research agents. I enjoy exploring how backend engineering and LLM technologies can work together to solve real-world problems.

## 🚀 Featured Projects

### 1. [Asynchronous AI Task Scheduling & Execution Platform](https://github.com/qianmu233/async-ai-task-platform)

**异步 AI 任务调度与执行平台**

`Java 17` `Spring Boot` `MySQL` `RabbitMQ` `Redis` `Lua`

- Builds an asynchronous task processing pipeline covering idempotent submission, persistent task states, background execution, and result retrieval.
- Implements Transactional Outbox, RabbitMQ Publisher Confirm/Return, conditional worker claims, and execution-token-based timeout protection.
- Integrates Mock and OpenAI-compatible model HTTP providers, with Redis Lua-based rate limiting.
- In a local benchmark with a 1000 ms Mock model and 8 concurrent requests, reduced task submission API p95 latency from **1019.125 ms to 2.245 ms**.

### 2. [Enterprise Knowledge Base & ERP Q&A Platform](https://github.com/qianmu233/enterprise-rag-erp-assistant)

**企业知识库与 ERP 智能问答平台**

`Java 17` `Spring AI` `RAG` `PostgreSQL` `PgVector` `ONNX Runtime` `SSE`

- Extends an open-source Spring AI project with PgVector-based knowledge retrieval and ERP tool calling for enterprise knowledge Q&A and business queries.
- Improves SSE streaming answer processing through cross-chunk buffering and incremental sanitization, filtering repeated internal markers while preserving structured ERP tool results.
- Adds model response and tool-calling protocol tests, together with fixed-dataset evaluation and offline retrieval experiments.
- Across three evaluation rounds on a 50-question dataset, reduced empty answers from **25/50 to 0/50** and improved literal key-fact phrase matching from **36.73% to 53.06%**.

Developed from [ly1836/spring-ai-rag-demo](https://github.com/ly1836/spring-ai-rag-demo), with project modifications and source boundaries documented in the repository.

### 3. [MCP Tool Invocation Security Gateway](https://github.com/qianmu233/agent-security-gateway)

**MCP 工具调用安全网关**

`Java` `Spring Security` `MCP` `API Key` `RBAC`

- Implements server-side API Key identity mapping and validates user roles, tenant boundaries, resource ownership, and tool permissions before execution.
- Introduces a one-time **Write Intent** mechanism with a 60-second expiration, binding authorization to the user, tool, tenant, order, and modification quantity.
- Uses a synchronized critical section to validate and consume authorization before updating Mock ERP order state, preventing concurrent replay within a single JVM.
- Validated through 24 MCP HTTP test scenarios: **8/8 authorized requests passed and 16/16 unauthorized requests were rejected**. Additional concurrency tests covered 280 requests, with 220 replay attempts rejected.

### 4. [ResearchPilot: Multi-Document Research & Citation Validation Agent](https://github.com/qianmu233/research-pilot)

**ResearchPilot：多文档智能研究与引用校验 Agent**

`Python` `FastAPI` `LangGraph` `RAG` `PgVector` `SQLite`

- Builds a five-node LangGraph workflow covering planning, retrieval, evidence assessment, report generation, and citation validation.
- Implements Chinese semantic retrieval using BGE-small-zh-v1.5 and validates citation source IDs and original excerpts against retrieved records.
- Persists task records with SQLite and workflow state with LangGraph Checkpointer, supporting controlled recovery with preserved model-call budgets and execution deadlines.
- On a small evaluation set of 19 synthetic documents and 16 answerable questions, improved Recall@5 from **53.125% to 100%** and MRR@5 from **51.04% to 96.875%**.

## 🛠️ Tech Stack

- **Languages:** Java · Python · SQL · C++
- **Backend & AI:** Spring Boot · Spring AI · FastAPI · LangGraph · RAG · MCP
- **Databases & Messaging:** MySQL · PostgreSQL · PgVector · Redis · RabbitMQ · SQLite
- **Testing & Infrastructure:** JUnit 5 · pytest · Docker · Maven · Git

## 🎯 Career Interests

Interested in internship opportunities in:

- Java Backend Engineering
- AI Platform Development
- LLM Application Development

Thanks for visiting my profile! 👋
