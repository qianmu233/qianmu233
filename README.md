# Hi, I'm Qianmu 👋

I'm a Software Engineering M.S. student at **South China Normal University**.

I focus on **Java backend engineering, AI platform development, and LLM application development**, with hands-on experience in asynchronous task processing, enterprise RAG, agent workflows, and secure tool integration.

I'm interested in building reliable backend systems and practical AI applications.

## 🚀 Featured Projects

### 1. [Asynchronous AI Task Orchestration Platform](https://github.com/qianmu233/async-ai-task-platform)

**异步 AI 任务调度与执行平台**

`Java 17` `Spring Boot` `MySQL` `RabbitMQ` `Redis`

- Provides asynchronous task submission, persistent task states, and idempotent request handling.
- Implements Transactional Outbox, RabbitMQ message dispatch, conditional worker claims, and timeout-safe result updates.
- Supports OpenAI-compatible model integration and optional Redis Lua rate limiting.

### 2. [Enterprise RAG & ERP Assistant](https://github.com/qianmu233/enterprise-rag-erp-assistant)

**企业级 RAG 与 ERP 智能业务助手**

`Spring AI` `RAG` `PostgreSQL` `PgVector` `ONNX Runtime` `SSE`

- Integrates enterprise document retrieval, knowledge-based question answering, and structured ERP data queries.
- Supports controlled tool calling, read-only SQL queries, session management, and SSE streaming responses.
- Developed from [ly1836/spring-ai-rag-demo](https://github.com/ly1836/spring-ai-rag-demo), with project modifications and source boundaries documented in the repository.

### 3. [ResearchPilot: Evidence-Grounded Research Agent](https://github.com/qianmu233/research-pilot)

**ResearchPilot：深度研究与证据溯源 Agent**

`Python` `FastAPI` `LangGraph` `RAG` `PgVector`

- Builds a multi-step research workflow covering planning, retrieval, evidence assessment, report generation, and citation validation.
- Implements Chinese semantic retrieval and source ID/excerpt validation against retrieved records.
- Persists task state and graph checkpoints, supporting task status queries and controlled manual recovery.

### 4. [Agent Tool Security Gateway](https://github.com/qianmu233/agent-security-gateway)

**Agent 工具调用安全授权网关**

`Java` `Spring Security` `MCP` `Python` `LangGraph`

- Connects a LangGraph agent to a Java MCP gateway for tool discovery and execution.
- Implements server-side identity mapping, RBAC, tenant and resource authorization, and one-time Write Intent validation.
- Includes replay protection, audit logging, and security tests based on a local Mock ERP environment.

## 🛠️ Tech Stack

- **Languages:** Java · Python · SQL · C++
- **Backend & AI:** Spring Boot · Spring AI · FastAPI · LangGraph · RAG · MCP
- **Databases & Messaging:** MySQL · PostgreSQL · PgVector · Redis · RabbitMQ
- **Tools & Infrastructure:** Docker · Maven · Git

## 🎯 Career Interests

Open to internship opportunities in:

- Java Backend Engineering
- AI Platform Development
- LLM Application Development

Thanks for visiting my profile!
