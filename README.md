# Hi, I'm Qianmu 👋

I'm a Software Engineering M.S. student at **South China Normal University**.

I focus on **Java backend engineering and LLM application development**, with interests in RAG, agent workflows, tool integration, and reliable asynchronous services.

## Featured Projects

### 1. [Asynchronous AI Task Orchestration Platform](https://github.com/qianmu233/async-ai-task-platform)
**异步 AI 任务调度与执行平台** · Java 17 · Spring Boot · MySQL · RabbitMQ · Redis

- Provides an asynchronous task API with persistent task states and idempotent submission.
- Uses Transactional Outbox for message dispatch, RabbitMQ consumers, conditional worker claims, and timeout-safe result updates.
- Includes an OpenAI-compatible model adapter and optional Redis Lua rate limiting.

### 2. [Enterprise RAG & ERP Assistant](https://github.com/qianmu233/enterprise-rag-erp-assistant)
**企业级 RAG 与 ERP 智能业务助手** · Spring AI · PostgreSQL/PgVector · ONNX Runtime · SSE

- Combines enterprise document retrieval and cited answers with structured ERP data queries.
- Supports controlled tool calling, read-only SQL, session management, and streaming responses.
- Developed from [ly1836/spring-ai-rag-demo](https://github.com/ly1836/spring-ai-rag-demo), with project changes and source boundaries documented in the repository.

### 3. [Agent Tool Security Gateway](https://github.com/qianmu233/agent-security-gateway)
**Agent 工具调用安全授权网关** · Spring Security · MCP · Python · LangGraph

- Connects a LangGraph agent to a Java MCP gateway for tool discovery and execution.
- Applies server-side authentication, RBAC, tenant/resource authorization, and checks for high-risk write operations before business execution.
- Uses inventory queries and purchase-order changes to demonstrate the authorization flow.

### 4. [ResearchPilot: Evidence-Grounded Research Agent](https://github.com/qianmu233/research-pilot)
**ResearchPilot：证据溯源深度研究智能体** · Python · FastAPI · LangGraph · RAG

- Organizes research into planning, retrieval, evidence assessment, and report generation.
- Checks report source IDs and excerpts against retrieved records, and exposes task status and execution traces.
- Persists task state and graph checkpoints for controlled manual recovery; supports Mock, local Ollama/Qwen, and cloud model backends.

## Tech Stack

- **Languages:** Java · Python · SQL · C++
- **Backend & AI:** Spring Boot · Spring AI · FastAPI · LangGraph · RAG · MCP
- **Data & Infrastructure:** MySQL · PostgreSQL · PgVector · Redis · RabbitMQ · Docker · Git

## Currently

Open to internship opportunities in **LLM Application Development and Backend Engineering**.
