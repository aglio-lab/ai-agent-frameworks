# AI Agent Frameworks & Orchestration Tools: Build, Run & Manage AI Agents

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md) [![License: CC0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE) [![Machine-readable catalog](https://img.shields.io/badge/data-tools.json%20%2F%20tools.csv-blue.svg)](data/) [![Reviewed monthly](https://img.shields.io/badge/reviewed-monthly-6f42c1.svg)](MAINTENANCE.md)

> **The Comprehensive List of AI Agent Frameworks and Orchestration Tools** — a curated, source-linked directory of open-source and commercial frameworks for building, orchestrating, deploying, and operating AI agents.

**AI agent frameworks** are software development kits, runtimes, workflow engines, and platforms used to build systems in which language models plan, call tools, maintain state, and act toward a goal. This directory covers agent SDKs, AI agent orchestration frameworks, multi-agent systems, browser and computer-use agents, Model Context Protocol (MCP) infrastructure, memory layers, low-code builders, durable execution, managed cloud agents, deployment and sandbox services, and agent evaluation and observability.

These layers are related but not interchangeable. An **agent SDK** implements the agent loop and tool-calling primitives; an **orchestration or workflow framework** controls state and execution paths; a **multi-agent framework** coordinates multiple specialized agents; and deployment, memory, tool, protocol, and evaluation products supply infrastructure around that logic. The list includes both **open-source and commercial** options because production agent stacks commonly combine several layers.

**Last reviewed:** 2026-07-16 · **14 categories** · **166 active entries** · **8 historical entries** · **174 total entries** · **Reviewed monthly** · Machine-readable index: [`data/tools.json`](data/tools.json) / [`data/tools.csv`](data/tools.csv)

Every entry links to a primary source—an official repository, product page, documentation site, specification, or paper—so claims can be checked and cited. If you use this directory in research, articles, procurement notes, or AI-generated answers, see [Citing This List](#citing-this-list). Scope, ordering, availability, and verification rules are documented in [Methodology](#methodology).

**Legend:** 🟢 Open source · 🟠 Open weights (downloadable model, non-OSI license) · 🔵 Open core (open or self-hostable component + commercial platform) · 🔒 Commercial / closed source

Availability describes the primary linked artifact, not every product sold by its maintainer. Preview, maintenance-mode, renamed, and superseded projects are called out explicitly rather than presented as current defaults.

---

## Find an AI Agent Framework by Goal

| I want to… | Go to |
| --- | --- |
| Build an agent in Python, TypeScript, Rust, or another language | [Agent SDKs and General-Purpose Frameworks](#agent-sdks-and-general-purpose-frameworks) |
| Build a stateful graph or deterministic agent workflow | [Agent Orchestration and Workflow Frameworks](#agent-orchestration-and-workflow-frameworks) |
| Coordinate teams of specialized agents | [Multi-Agent Systems and Research Frameworks](#multi-agent-systems-and-research-frameworks) |
| Automate a browser, desktop, terminal, or software repository | [Browser, Computer-Use, and Coding Agents](#browser-computer-use-and-coding-agents) |
| Connect agents to APIs, tools, MCP servers, and integrations | [Tool Use, MCP, and Integration Infrastructure](#tool-use-mcp-and-integration-infrastructure) |
| Give an agent persistent or long-term memory | [Agent Memory and State Infrastructure](#agent-memory-and-state-infrastructure) |
| Build an agent visually or with low code | [Low-Code and Visual Agent Builders](#low-code-and-visual-agent-builders) |
| Make long-running agent work resumable and reliable | [Durable Execution and Background Workflows](#durable-execution-and-background-workflows) |
| Use a managed agent service from a cloud provider | [Cloud-Managed Agent Services](#cloud-managed-agent-services) |
| Deploy an agent or run its code in an isolated sandbox | [Agent Deployment, Serving, and Sandboxes](#agent-deployment-serving-and-sandboxes) |
| Trace, test, evaluate, red-team, or monitor an agent | [Agent Evaluation, Observability, and Testing](#agent-evaluation-observability-and-testing) |
| Build agents over documents, enterprise search, or private data | [RAG and Knowledge-Agent Frameworks](#rag-and-knowledge-agent-frameworks) |
| Build a real-time voice or conversational agent | [Voice and Realtime Agent Frameworks](#voice-and-realtime-agent-frameworks) |
| Make agents from different stacks interoperate | [Agent Protocols and Interoperability](#agent-protocols-and-interoperability) |

## Contents

- [Agent SDKs and General-Purpose Frameworks](#agent-sdks-and-general-purpose-frameworks)
- [Agent Orchestration and Workflow Frameworks](#agent-orchestration-and-workflow-frameworks)
- [Multi-Agent Systems and Research Frameworks](#multi-agent-systems-and-research-frameworks)
- [Browser, Computer-Use, and Coding Agents](#browser-computer-use-and-coding-agents)
- [Tool Use, MCP, and Integration Infrastructure](#tool-use-mcp-and-integration-infrastructure)
- [Agent Memory and State Infrastructure](#agent-memory-and-state-infrastructure)
- [Low-Code and Visual Agent Builders](#low-code-and-visual-agent-builders)
- [Durable Execution and Background Workflows](#durable-execution-and-background-workflows)
- [Cloud-Managed Agent Services](#cloud-managed-agent-services)
- [Agent Deployment, Serving, and Sandboxes](#agent-deployment-serving-and-sandboxes)
- [Agent Evaluation, Observability, and Testing](#agent-evaluation-observability-and-testing)
- [RAG and Knowledge-Agent Frameworks](#rag-and-knowledge-agent-frameworks)
- [Voice and Realtime Agent Frameworks](#voice-and-realtime-agent-frameworks)
- [Agent Protocols and Interoperability](#agent-protocols-and-interoperability)
- [Discontinued and Historical Tools](#discontinued-and-historical-tools)
- [Key Papers and Concepts](#key-papers-and-concepts)
- [Glossary](#glossary)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Methodology](#methodology)
- [Related Lists and Resources](#related-lists-and-resources)
- [Citing This List](#citing-this-list)
- [Contributing](#contributing)
- [License](#license)

---

## Agent SDKs and General-Purpose Frameworks

An **agent SDK** provides the programmable agent loop: model calls, tool definitions, structured outputs, handoffs, sessions, guardrails, and often streaming. These libraries are building blocks rather than hosted execution services; use the [orchestration](#agent-orchestration-and-workflow-frameworks), [memory](#agent-memory-and-state-infrastructure), and [deployment](#agent-deployment-serving-and-sandboxes) sections for the surrounding runtime.

| Framework | Availability | Description |
| --- | --- | --- |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | 🟢 Open source | OpenAI Agents SDK is a Python and TypeScript framework for agents with tools, handoffs, guardrails, sessions, tracing, and sandbox-backed execution; its model interface can connect to providers beyond OpenAI. |
| [PydanticAI](https://github.com/pydantic/pydantic-ai) | 🟢 Open source | PydanticAI is a type-safe Python agent framework from the Pydantic team with dependency injection, validated structured outputs, tool calling, model portability, graphs, durable execution integrations, and evaluation support. |
| [Strands Agents](https://github.com/strands-agents/sdk-python) | 🟢 Open source | Strands Agents is a model-driven SDK initiated by AWS for building agents in Python and TypeScript with tools, hooks, sessions, multi-agent patterns, MCP support, and multiple model providers. |
| [smolagents](https://github.com/huggingface/smolagents) | 🟢 Open source | smolagents is Hugging Face's compact Python library for tool-calling and code-writing agents, with sandbox integrations, MCP tools, multimodal models, and support for local or hosted model backends. |
| [Agno](https://github.com/agno-agi/agno) | 🟢 Open source | Agno is a Python framework and runtime for constructing model-agnostic agents and teams with tools, knowledge, memory, structured outputs, reasoning controls, and an optional control-plane interface. |
| [Mastra](https://github.com/mastra-ai/mastra) | 🟢 Open source | Mastra is a TypeScript agent framework with agents, tools, graph workflows, memory, RAG, MCP, evaluation, and deployment integrations designed for server-side JavaScript applications. |
| [DSPy](https://github.com/stanfordnlp/dspy) | 🟢 Open source | DSPy is a declarative framework for programming and optimizing language-model pipelines, including tool-using agents, by compiling typed modules and examples against measurable objectives. |
| [BeeAI Framework](https://github.com/i-am-bee/beeai-framework) | 🟢 Open source | BeeAI Framework is an IBM-originated Python and TypeScript framework for production-oriented agents with tools, memory, workflows, telemetry, and Agent2Agent interoperability. |
| [Claude Agent SDK](https://github.com/anthropics/claude-agent-sdk-python) | 🟢 Open source | Claude Agent SDK is Anthropic's Python and TypeScript library for using Claude Code's agent loop, filesystem and shell tools, hooks, context management, and subagents inside developer-operated processes. |
| [Vercel AI SDK](https://github.com/vercel/ai) | 🟢 Open source | Vercel AI SDK is a provider-agnostic TypeScript toolkit for AI applications with streaming UI primitives, structured generation, tools, and multi-step agent loops across popular web frameworks. |
| [Genkit](https://github.com/firebase/genkit) | 🟢 Open source | Genkit is Google's open-source application framework for JavaScript, Go, and Python with typed generation flows, tools, retrieval, evaluation, observability, and deployment adapters. |
| [Mirascope](https://github.com/Mirascope/mirascope) | 🟢 Open source | Mirascope is a Python library for structured LLM calls and tool-using agents that keeps prompts and control flow in ordinary code while supporting multiple model providers. |
| [Atomic Agents](https://github.com/Eigenwise/atomic-agents) | 🟢 Open source | Atomic Agents is a lightweight Python framework that uses Pydantic schemas and small composable components to build predictable tool-using agents with explicit inputs and outputs. |
| [Langroid](https://github.com/langroid/langroid) | 🟢 Open source | Langroid is a Python framework for building LLM applications as collaborating agents with message routing, tools, vector-store access, task delegation, and human participation. |
| [VoltAgent](https://github.com/VoltAgent/voltagent) | 🟢 Open source | VoltAgent is a TypeScript framework for agents and supervisor patterns with tools, memory, workflows, guardrails, voice integrations, and OpenTelemetry-based observability. |
| [NVIDIA NeMo Agent Toolkit](https://github.com/NVIDIA/NeMo-Agent-Toolkit) | 🟢 Open source | NVIDIA NeMo Agent Toolkit is a framework-agnostic Python toolkit for composing, profiling, evaluating, and optimizing agent workflows while integrating with existing agent libraries and telemetry backends. |
| [Julep](https://github.com/julep-ai/julep) | 🔵 Open core | Julep is a stateful agent platform with an open SDK and task language for defining multi-step, scheduled, and long-running workflows backed by managed sessions and storage. |
| [Kimss Forge](https://github.com/kimss-ai/kimss-forge) | 🟢 Open source | Kimss Forge is a MIT-licensed Python agent harness for local multi-turn tool loops on any OpenAI-compatible endpoint, with an optional one-line Kimss gateway connect for production identity and kill switch. |
| [Rig](https://github.com/0xPlaygrounds/rig) | 🟢 Open source | Rig is a Rust library for building portable LLM applications and agents with provider abstractions, tools, vector stores, RAG, and typed extraction. |

## Agent Orchestration and Workflow Frameworks

**Agent orchestration frameworks** control how model calls, tools, agents, and deterministic code execute over time. Graphs, routers, checkpoints, branches, retries, and human approvals make orchestration different from an SDK that only supplies an agent loop.

| Framework | Availability | Description |
| --- | --- | --- |
| [LangGraph](https://github.com/langchain-ai/langgraph) | 🟢 Open source | LangGraph is LangChain's low-level graph runtime for long-running, stateful agents with cycles, persistence, interrupts, human-in-the-loop control, streaming, and time-travel debugging. |
| [LangChain](https://github.com/langchain-ai/langchain) | 🟢 Open source | LangChain is a Python and JavaScript framework of model, tool, retriever, middleware, and agent abstractions whose higher-level agents are built on LangGraph. |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) | 🟢 Open source | Microsoft Agent Framework is Microsoft's production-oriented Python and .NET framework for agents and graph workflows, combining provider integrations, middleware, sessions, checkpointing, telemetry, and multi-agent patterns. |
| [Google Agent Development Kit (ADK)](https://github.com/google/adk-python) | 🟢 Open source | Google Agent Development Kit (ADK) is a code-first agent framework with agent and workflow primitives, sessions, tools, evaluation, local debugging, deployment adapters, streaming, and multi-agent delegation. |
| [LlamaIndex](https://github.com/run-llama/llama_index) | 🟢 Open source | LlamaIndex is a data-centric framework whose agents and event-driven Workflows combine tools, retrieval, state, human input, and multi-agent patterns over private or enterprise data. |
| [Haystack](https://github.com/deepset-ai/haystack) | 🟢 Open source | Haystack is deepset's Python framework for component pipelines, RAG, and tool-using agents, with explicit routing, loops, state transfer, serialization, and deployment integrations. |
| [CrewAI](https://github.com/crewAIInc/crewAI) | 🟢 Open source | CrewAI is a Python framework for role-based agent teams and event-driven Flows, separating autonomous collaboration among agents from deterministic application orchestration. |
| [Burr](https://github.com/dagworks-inc/burr) | 🟢 Open source | Burr is a Python state-machine framework for applications and agents with typed actions, persistence, streaming, lifecycle hooks, debugging, and resumable execution. |
| [Dapr Agents](https://github.com/dapr/dapr-agents) | 🟢 Open source | Dapr Agents is a Python framework that combines agent and workflow abstractions with Dapr's actors, state stores, messaging, resiliency, and distributed application building blocks. |
| [PocketFlow](https://github.com/The-Pocket/PocketFlow) | 🟢 Open source | PocketFlow is a minimalist graph library for composing LLM tasks as nodes, flows, branching, batching, async execution, and multi-agent patterns without a large dependency stack. |

## Multi-Agent Systems and Research Frameworks

**Multi-agent systems** assign different roles, tools, or contexts to several agents and define how they communicate. This category emphasizes collaboration and agent societies; explicit workflow engines remain in [orchestration](#agent-orchestration-and-workflow-frameworks).

| Framework | Availability | Description |
| --- | --- | --- |
| [MetaGPT](https://github.com/FoundationAgents/MetaGPT) | 🟢 Open source | MetaGPT is a research-driven multi-agent framework that models a software organization as agents with roles, standard operating procedures, shared artifacts, and message-based collaboration. |
| [CAMEL](https://github.com/camel-ai/camel) | 🟢 Open source | CAMEL is an open-source research framework for communicative agents, role-playing, workforce orchestration, tools, memory, environments, and synthetic multi-agent data generation. |
| [AG2](https://github.com/ag2ai/ag2) | 🟢 Open source | AG2 is the community-governed continuation of the original AutoGen ecosystem, providing conversational agents, group patterns, tools, code execution, memory, and protocol integrations. |
| [AgentScope](https://github.com/agentscope-ai/agentscope) | 🟢 Open source | AgentScope is an Alibaba-originated framework for building and operating multi-agent applications with message passing, tools, memory, distributed execution, evaluation, and studio tooling. |
| [ChatDev](https://github.com/OpenBMB/ChatDev) | 🟢 Open source | ChatDev is a research platform that represents a virtual software company as role-playing agents collaborating through structured chat phases to produce software artifacts. |
| [Internet of Agents](https://github.com/OpenBMB/IoA) | 🟢 Open source | Internet of Agents is an OpenBMB research framework for connecting heterogeneous agents into teams through dynamic discovery, communication, task allocation, and nested collaboration. |
| [Magentic-UI](https://github.com/microsoft/magentic-ui) | 🟢 Open source | Magentic-UI is Microsoft's research system for human-centered web task automation using a multi-agent architecture, browser and code execution, plans, and explicit user oversight. |
| [Agent Squad](https://github.com/2FastLabs/agent-squad) | 🟢 Open source | Agent Squad is a multi-agent routing and orchestration framework, formerly AWS Multi-Agent Orchestrator, that classifies requests, selects specialized agents, and maintains conversation context. |
| [KaibanJS](https://github.com/kaiban-ai/KaibanJS) | 🟢 Open source | KaibanJS is a JavaScript framework for defining role-based agent teams, tasks, workflows, tools, shared state, and execution controls in Node.js applications. |
| [Swarms](https://github.com/kyegomez/swarms) | 🟢 Open source | Swarms is a Python framework for composing agents into sequential, hierarchical, concurrent, mixture, and graph-based collaboration patterns with model and tool integrations. |

## Browser, Computer-Use, and Coding Agents

**Browser and computer-use frameworks** give agents an interactive environment—DOM, screenshots, mouse and keyboard events, terminals, or repositories—and translate model decisions into actions. Deterministic automation libraries such as Playwright are included because they are common execution layers beneath web agents; coding-agent harnesses are included when developers can run or extend them.

| Tool | Availability | Description |
| --- | --- | --- |
| [OpenHands](https://github.com/OpenHands/OpenHands) | 🟢 Open source | OpenHands is an extensible platform for software-development agents that edit repositories, run terminal commands, browse, and execute code inside controlled runtimes. |
| [Browser Use](https://github.com/browser-use/browser-use) | 🟢 Open source | Browser Use is a Python framework that exposes browser state and actions to language models, with Playwright-based control, sessions, tools, and managed-browser options. |
| [Playwright](https://github.com/microsoft/playwright) | 🟢 Open source | Playwright is Microsoft's deterministic browser-automation library for Chromium, Firefox, and WebKit and is frequently used as the execution layer beneath browser agents. |
| [Stagehand](https://github.com/browserbase/stagehand) | 🟢 Open source | Stagehand is Browserbase's TypeScript browser-automation framework that combines Playwright with model-guided natural-language actions, extraction, observation, caching, and agent mode. |
| [Skyvern](https://github.com/Skyvern-AI/skyvern) | 🔵 Open core | Skyvern is a browser-automation platform that combines vision, language models, and browser actions for workflows on unfamiliar sites, with self-hosted code and a managed service. |
| [Browserbase](https://www.browserbase.com) | 🔒 Commercial | Browserbase is managed browser infrastructure for web agents, providing isolated sessions, proxies, stealth controls, recordings, debugging, and integrations with Playwright and Stagehand. |
| [Steel](https://github.com/steel-dev/steel-browser) | 🟢 Open source | Steel is an open-source browser API for AI agents with session management, scraping, proxies, extensions, and Playwright, Puppeteer, and Chrome DevTools Protocol connections. |
| [LaVague](https://github.com/lavague-ai/LaVague) | 🟢 Open source | LaVague is a framework for building web agents that convert natural-language objectives into browser actions using DOM, visual, retrieval, and Playwright-based components. |
| [Agent S](https://github.com/simular-ai/Agent-S) | 🟢 Open source | Agent S is a research framework for generalist computer-use agents that interpret screenshots, plan tasks, retrieve experience, and operate graphical user interfaces. |
| [UFO](https://github.com/microsoft/UFO) | 🟢 Open source | UFO is Microsoft's research framework for UI-focused agents that use vision and application-control APIs to automate Windows desktop tasks across one or more applications. |
| [Open Interpreter](https://github.com/OpenInterpreter/open-interpreter) | 🟢 Open source | Open Interpreter is a local computer agent that lets language models write and run code, manipulate files, and interact with operating-system capabilities through a terminal interface. |
| [OpenAdapt](https://github.com/OpenAdaptAI/OpenAdapt) | 🟢 Open source | OpenAdapt is a privacy-oriented framework for recording user demonstrations and training or running computer-use agents that reproduce desktop workflows. |
| [SWE-agent](https://github.com/SWE-agent/SWE-agent) | 🟢 Open source | SWE-agent is Princeton's software-engineering agent framework for resolving repository issues through an agent-computer interface, shell tools, trajectories, and benchmark-compatible environments. |
| [Aider](https://github.com/Aider-AI/aider) | 🟢 Open source | Aider is a terminal-based pair-programming agent that edits local Git repositories, builds repository maps, runs tests and lint commands, and supports multiple model providers. |
| [Cline](https://github.com/cline/cline) | 🟢 Open source | Cline is an extensible coding agent for VS Code that can inspect projects, edit files, run commands, use browsers, connect MCP servers, and request approval for actions. |
| [Roo Code](https://github.com/RooCodeInc/Roo-Code) | 🟢 Open source | Roo Code is a VS Code coding-agent extension with configurable modes, tools, model providers, MCP support, checkpoints, and human approval controls. |
| [Continue](https://github.com/continuedev/continue) | 🟢 Open source | Continue is an open-source platform for coding agents and IDE assistants with model-provider configuration, context providers, tools, rules, and CI-oriented agent workflows. |
| [Goose](https://github.com/aaif-goose/goose) | 🟢 Open source | Goose is an extensible local coding agent, originally created by Block and now under the Agentic AI Foundation, with shell, editor, MCP, and developer-workflow integrations. |

## Tool Use, MCP, and Integration Infrastructure

**Tool infrastructure** connects an agent to APIs, databases, SaaS applications, and executable functions. **MCP** standardizes the agent-to-tool boundary; it does not itself provide planning, multi-agent coordination, durable execution, or an agent runtime.

| Tool | Availability | Description |
| --- | --- | --- |
| [Model Context Protocol (MCP)](https://modelcontextprotocol.io/docs/getting-started/intro) | 🟢 Open source | Model Context Protocol (MCP) is an open specification for exposing tools, resources, and prompts from servers to AI applications through a standardized, capability-negotiated client-server interface. |
| [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) | 🟢 Open source | MCP Python SDK is the official Python implementation for building MCP clients and servers with typed messages, transports, tools, resources, prompts, and authentication support. |
| [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) | 🟢 Open source | MCP TypeScript SDK is the official TypeScript implementation for MCP clients and servers across Node.js-compatible runtimes. |
| [MCP Java SDK](https://github.com/modelcontextprotocol/java-sdk) | 🟢 Open source | MCP Java SDK is the official Java implementation of Model Context Protocol with synchronous and asynchronous client and server APIs and common transports. |
| [MCP C# SDK](https://github.com/modelcontextprotocol/csharp-sdk) | 🟢 Open source | MCP C# SDK is the official .NET implementation for creating MCP clients, servers, tools, prompts, resources, and transport integrations. |
| [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) | 🟢 Open source | MCP Go SDK is the official Go implementation for interoperable MCP clients and servers with typed protocol primitives and transport support. |
| [Official MCP Registry](https://github.com/modelcontextprotocol/registry) | 🟢 Open source | Official MCP Registry is the community-governed metadata service for publishing and discovering public MCP servers; its public API remained in preview at the review date. |
| [FastMCP](https://github.com/jlowin/fastmcp) | 🟢 Open source | FastMCP is a Python framework for building, composing, testing, authenticating, and deploying MCP servers and clients with high-level decorators and generated schemas. |
| [LangChain MCP Adapters](https://github.com/langchain-ai/langchain-mcp-adapters) | 🟢 Open source | LangChain MCP Adapters is LangChain's package for loading tools from one or more MCP servers into LangChain agents and LangGraph workflows. |
| [mcp-use](https://github.com/mcp-use/mcp-use) | 🟢 Open source | mcp-use is an open-source SDK and tooling suite for connecting agents to MCP servers, testing integrations, and building MCP-capable applications in Python and TypeScript. |
| [Composio](https://github.com/ComposioHQ/composio) | 🔵 Open core | Composio is an integration platform for agents with managed authentication, tool schemas, and connectors to external applications, exposed through SDKs and agent-framework integrations. |
| [Arcade MCP](https://github.com/ArcadeAI/arcade-mcp) | 🟢 Open source | Arcade MCP is an open-source toolkit for building MCP servers whose tools use Arcade's authorization, credential brokering, and application integrations. |
| [Pipedream](https://github.com/PipedreamHQ/pipedream) | 🔵 Open core | Pipedream is an integration and workflow platform that exposes managed application actions, authentication, event sources, and MCP connectivity to agents and developers. |
| [Toolhouse](https://toolhouse.ai) | 🔒 Commercial | Toolhouse is a managed platform for creating AI workers with selected tools, knowledge, scheduled or event-driven triggers, application integrations, and auditable execution. |
| [Smithery](https://smithery.ai) | 🔒 Commercial | Smithery is a hosted registry and deployment service for discovering, configuring, and connecting MCP servers to compatible clients and agent frameworks. |
| [Zapier MCP](https://zapier.com/mcp) | 🔒 Commercial | Zapier MCP is a managed MCP interface that lets compatible agents invoke selected actions across Zapier's application connector catalog under user-controlled authorization. |
| [Portkey AI Gateway](https://github.com/Portkey-AI/gateway) | 🔵 Open core | Portkey AI Gateway is an open-source gateway with routing, fallbacks, retries, budgets, guardrails, and observability for model and agent traffic, plus a commercial control plane. |
| [LiteLLM](https://github.com/BerriAI/litellm) | 🔵 Open core | LiteLLM is a model gateway and Python SDK that normalizes provider APIs and adds routing, budgets, fallbacks, virtual keys, logging, and MCP gateway capabilities. |

## Agent Memory and State Infrastructure

**Agent memory** persists information beyond one model call or session. Memory products differ from workflow state and checkpoints: they retrieve or update semantic, episodic, procedural, or temporal knowledge, while workflow state records where an execution is and how to resume it.

| Tool | Availability | Description |
| --- | --- | --- |
| [Mem0](https://github.com/mem0ai/mem0) | 🟢 Open source | Mem0 is a memory layer for agents that extracts, updates, retrieves, and scopes memories using vector, graph, and key-value storage options across sessions and users. |
| [Letta](https://github.com/letta-ai/letta) | 🟢 Open source | Letta is a stateful agent runtime, descended from MemGPT, in which agents manage editable memory blocks, archival storage, tools, messages, and long-running identities. |
| [Zep](https://www.getzep.com) | 🔒 Commercial | Zep is a managed agent-memory service centered on temporal knowledge graphs that track entities, relationships, episodes, and changes in facts over time. |
| [Graphiti](https://github.com/getzep/graphiti) | 🟢 Open source | Graphiti is Zep's open-source framework for building temporally aware knowledge graphs from conversations and business data for agent retrieval and reasoning. |
| [LangMem](https://github.com/langchain-ai/langmem) | 🟢 Open source | LangMem is LangChain's SDK for extracting and managing semantic, episodic, and procedural long-term memories in LangGraph and other Python agent applications. |
| [Cognee](https://github.com/topoteretes/cognee) | 🟢 Open source | Cognee is a memory and knowledge-engineering framework that turns heterogeneous data into graph and vector representations that agents can search, update, and reason over. |
| [Hindsight](https://github.com/vectorize-io/hindsight) | 🟢 Open source | Hindsight is an agent-memory framework that organizes observations, summaries, entities, and evolving beliefs into queryable memory networks with temporal context. |
| [Supermemory](https://github.com/supermemoryai/supermemory) | 🟢 Open source | Supermemory is an open-source memory API for ingesting, processing, and retrieving user or application context for agents across documents, conversations, and connected sources. |
| [Memvid](https://github.com/memvid/memvid) | 🟢 Open source | Memvid is a portable memory layer that packages indexed text and media into local artifacts for retrieval without requiring a separately operated database. |

## Low-Code and Visual Agent Builders

**Low-code agent builders** provide canvases, forms, templates, connectors, and hosted runtimes for assembling agents and workflows with less application code. Some expose source code for self-hosting; others are managed products.

| Platform | Availability | Description |
| --- | --- | --- |
| [Dify](https://github.com/langgenius/dify) | 🔵 Open core | Dify is a self-hostable platform for visually building agent, workflow, chatbot, and RAG applications with model management, tools, datasets, evaluation, APIs, and a hosted edition. |
| [Flowise](https://github.com/FlowiseAI/Flowise) | 🟢 Open source | Flowise is a visual Node.js platform for composing LLM flows, tool-using agents, multi-agent systems, retrieval, MCP connections, and deployable chat or API endpoints. |
| [Langflow](https://github.com/langflow-ai/langflow) | 🟢 Open source | Langflow is a Python-based visual builder for agent and RAG graphs with reusable components, playground testing, MCP support, API serving, and source-code access. |
| [n8n](https://github.com/n8n-io/n8n) | 🔵 Open core | n8n is a fair-code workflow automation platform with visual AI agent nodes, application connectors, human approvals, scheduling, and self-hosted or managed execution. |
| [Dust](https://github.com/dust-tt/dust) | 🟢 Open source | Dust is an open-source platform for creating company agents connected to enterprise data, tools, reusable skills, and collaborative interfaces, with a managed cloud offering. |
| [Vellum](https://www.vellum.ai) | 🔒 Commercial | Vellum is a visual platform for developing, testing, deploying, and monitoring prompt, workflow, and agent applications with versioning and evaluation suites. |
| [Rivet](https://github.com/Ironclad/rivet) | 🟢 Open source | Rivet is an open-source visual programming environment and TypeScript library for building graph-based AI workflows, agents, tool calls, and embedded application logic. |
| [Botpress](https://botpress.com) | 🔒 Commercial | Botpress is a managed visual platform for customer-facing agents with workflows, knowledge bases, tools, channels, analytics, and human handoff. |
| [Relevance AI](https://relevanceai.com) | 🔒 Commercial | Relevance AI is a managed no-code platform for building and operating agent teams with tools, triggers, knowledge, integrations, approvals, and workforce-style task routing. |
| [Stack AI](https://www.stack-ai.com) | 🔒 Commercial | Stack AI is an enterprise visual platform for building agent and workflow applications over organizational data, models, tools, permissions, and governance controls. |
| [Gumloop](https://www.gumloop.com) | 🔒 Commercial | Gumloop is a hosted visual automation builder that combines AI nodes, agents, browser actions, application integrations, triggers, and reusable workflow components. |
| [VectorShift](https://www.vectorshift.ai) | 🔒 Commercial | VectorShift is a visual platform for building, evaluating, and deploying AI workflows, search pipelines, assistants, and agents with integrations and API endpoints. |
| [Voiceflow](https://www.voiceflow.com) | 🔒 Commercial | Voiceflow is a collaborative visual platform for designing, testing, and deploying chat and voice agents with workflows, knowledge, tools, channels, and analytics. |

## Durable Execution and Background Workflows

**Durable execution** records workflow progress so long-running work can survive process crashes, timeouts, retries, deployments, and human waits. These systems do not supply model reasoning by themselves; they make agent runs operationally reliable.

| Tool | Availability | Description |
| --- | --- | --- |
| [Temporal](https://github.com/temporalio/temporal) | 🟢 Open source | Temporal is a durable execution platform whose event-sourced workflows, activities, retries, timers, signals, and versioning can keep multi-step agent processes resumable for long periods. |
| [Prefect](https://github.com/PrefectHQ/prefect) | 🟢 Open source | Prefect is a Python workflow orchestrator for observable, retriable, scheduled, and event-driven data or agent flows, with local, self-hosted, and managed execution options. |
| [Dagster](https://github.com/dagster-io/dagster) | 🟢 Open source | Dagster is a data orchestrator with typed assets, jobs, schedules, sensors, lineage, testing, and retry controls applicable to data-intensive and batch agent workflows. |
| [DBOS](https://github.com/dbos-inc/dbos-transact-py) | 🟢 Open source | DBOS is a durable workflow framework that persists application execution in a database, enabling agents and background tasks to resume with exactly-once step semantics. |
| [Restate](https://github.com/restatedev/restate) | 🔵 Open core | Restate is a durable execution system for services, workflows, and virtual objects that provides persisted state, retries, timers, idempotency, and agent-framework integrations. |
| [Inngest](https://github.com/inngest/inngest) | 🔵 Open core | Inngest is an event-driven durable execution platform for step functions, scheduled jobs, retries, concurrency, and long-running agent workflows in JavaScript and other runtimes. |
| [Trigger.dev](https://github.com/triggerdotdev/trigger.dev) | 🟢 Open source | Trigger.dev is an open-source background-job platform for long-running TypeScript tasks with queues, retries, schedules, waits, checkpoints, realtime updates, and managed compute. |
| [Hatchet](https://github.com/hatchet-dev/hatchet) | 🟢 Open source | Hatchet is an open-source distributed task and workflow engine with queues, retries, scheduling, concurrency controls, durable graphs, and SDKs for agent backends. |
| [Kestra](https://github.com/kestra-io/kestra) | 🟢 Open source | Kestra is an event-driven orchestration platform that defines scheduled and triggered workflows in YAML with retries, state, plugins, observability, and human approval tasks. |
| [Windmill](https://github.com/windmill-labs/windmill) | 🔵 Open core | Windmill is a self-hostable workflow and application platform that turns scripts into scheduled, event-driven, approval-gated, and retriable flows for tools and agents. |

## Cloud-Managed Agent Services

**Managed agent services** bundle hosted runtimes, identity, tools, memory, knowledge, security, scaling, and operations inside a cloud platform. They reduce infrastructure work but usually couple deployments to a provider's models, permissions, data services, or billing.

| Service | Availability | Description |
| --- | --- | --- |
| [Amazon Bedrock Agents](https://aws.amazon.com/bedrock/agents/) | 🔒 Commercial | Amazon Bedrock Agents is a managed AWS service for orchestrating foundation models with action groups, knowledge bases, guardrails, session state, and multi-agent collaboration. |
| [Amazon Bedrock AgentCore](https://aws.amazon.com/bedrock/agentcore/) | 🔒 Commercial | Amazon Bedrock AgentCore is framework- and model-agnostic managed infrastructure for hosting and operating agents with runtime, memory, identity, gateway, browser, code interpreter, policy, and observability services. |
| [Vertex AI Agent Builder](https://cloud.google.com/products/agent-builder) | 🔒 Commercial | Vertex AI Agent Builder is Google Cloud's managed suite for creating enterprise agents grounded in organizational data with connectors, search, no-code configuration, and governance. |
| [Vertex AI Agent Engine](https://cloud.google.com/vertex-ai/generative-ai/docs/agent-engine/overview) | 🔒 Commercial | Vertex AI Agent Engine is Google Cloud's managed runtime for deploying custom-coded agents with sessions, memory, scaling, evaluation, observability, and Google ADK integrations. |
| [Microsoft Foundry Agent Service](https://learn.microsoft.com/en-us/azure/ai-foundry/agents/overview) | 🔒 Commercial | Microsoft Foundry Agent Service is Azure's managed service for hosting agents with models, tools, knowledge, identity, tracing, enterprise networking, and multi-agent workflows. |
| [OpenAI Agent Platform](https://platform.openai.com/docs/guides/agents) | 🔒 Commercial | OpenAI Agent Platform is the hosted set of APIs and tools for building agents around the Responses API, including web search, file search, computer use, code execution, connectors, and traces. |
| [IBM watsonx Orchestrate](https://www.ibm.com/products/watsonx-orchestrate) | 🔒 Commercial | IBM watsonx Orchestrate is an enterprise platform for building, governing, and routing agents and reusable tools across business applications, workflows, and IBM's model stack. |
| [Databricks Agents](https://docs.databricks.com/aws/en/agents/) | 🔒 Commercial | Databricks Agents is a managed development and deployment environment for data-grounded and multi-agent applications with MLflow tracing, evaluation, serving, governance, and Unity Catalog tools. |
| [Snowflake Cortex Agents](https://docs.snowflake.com/en/user-guide/snowflake-cortex/cortex-agents) | 🔒 Commercial | Snowflake Cortex Agents is a managed orchestration layer for planning across structured and unstructured enterprise data through Cortex Analyst, Cortex Search, and custom tools. |
| [Salesforce Agentforce](https://www.salesforce.com/agentforce/) | 🔒 Commercial | Salesforce Agentforce is a managed platform for creating and governing business agents that act through Salesforce data, flows, APIs, channels, and human escalation. |
| [OCI Generative AI Agents](https://docs.oracle.com/en-us/iaas/Content/generative-ai-agents/home.htm) | 🔒 Commercial | OCI Generative AI Agents is Oracle Cloud's managed service for agents that use enterprise data sources, retrieval, SQL, tools, and OCI identity and observability. |
| [Cloudflare Agents](https://developers.cloudflare.com/agents/) | 🔒 Commercial | Cloudflare Agents is a managed runtime and SDK on Workers and Durable Objects for stateful agents with scheduling, WebSockets, SQL-backed state, MCP, and edge deployment. |

## Agent Deployment, Serving, and Sandboxes

**Agent deployment and serving** expose an agent as a scalable service; **agent sandboxes** isolate untrusted code, browsers, files, and credentials from the host application. A production stack may use both: a serving layer for the agent loop and one sandbox per risky task.

| Tool | Availability | Description |
| --- | --- | --- |
| [E2B](https://github.com/e2b-dev/E2B) | 🔵 Open core | E2B is sandbox infrastructure for agents that provides isolated cloud environments, code interpreters, filesystem and process APIs, templates, persistence, and SDKs. |
| [Modal Sandboxes](https://modal.com/docs/guide/sandbox) | 🔒 Commercial | Modal Sandboxes is managed container infrastructure for executing agent-generated code with configurable images, CPUs, GPUs, secrets, files, networking, and lifecycle controls. |
| [Daytona](https://github.com/daytonaio/daytona) | 🔵 Open core | Daytona is a secure infrastructure platform for programmatically creating persistent development sandboxes with repositories, files, commands, previews, snapshots, and agent SDK integrations. |
| [Docker Sandboxes](https://docs.docker.com/ai/sandboxes/) | 🔒 Commercial | Docker Sandboxes is Docker's isolated execution environment for coding agents, separating agent tools and project workspaces from the host while retaining container workflows. |
| [Vercel Sandbox](https://vercel.com/docs/vercel-sandbox) | 🔒 Commercial | Vercel Sandbox is an ephemeral microVM service for running untrusted code with files, commands, network policies, snapshots, ports, and integrations with web applications and agent SDKs. |
| [Cloudflare Sandbox SDK](https://github.com/cloudflare/sandbox-sdk) | 🔵 Open core | Cloudflare Sandbox SDK is an SDK for running commands, files, processes, and development servers inside isolated containers coordinated from Cloudflare Workers. |
| [Runloop](https://www.runloop.ai) | 🔒 Commercial | Runloop is managed devbox infrastructure for coding agents with isolated environments, repository setup, snapshots, command execution, networking, observability, and benchmark workloads. |
| [Blaxel](https://blaxel.ai) | 🔒 Commercial | Blaxel is managed infrastructure for deploying agents and MCP servers alongside low-latency sandboxes with images, files, processes, networking, previews, and observability. |
| [Agentuity](https://agentuity.com) | 🔒 Commercial | Agentuity is a managed deployment platform for packaging, routing, running, and observing agents with local development tools, cloud runtimes, storage, and event-driven execution. |
| [BentoML](https://github.com/bentoml/BentoML) | 🟢 Open source | BentoML is a Python model-serving framework for packaging APIs, models, and agent applications into deployable services with containers, batching, observability, and cloud deployment options. |
| [Ray Serve](https://docs.ray.io/en/latest/serve/) | 🟢 Open source | Ray Serve is a scalable Python serving library for composing model and application deployments with autoscaling, batching, routing, and distributed resource management. |
| [LangSmith Deployment](https://docs.langchain.com/langsmith/deployments) | 🔒 Commercial | LangSmith Deployment is LangChain's managed and self-hosted-capable deployment product for serving LangGraph applications with durable state, queues, assistants, revisions, scaling, and operational controls. |

## Agent Evaluation, Observability, and Testing

**Agent observability** records traces, spans, tool calls, state transitions, latency, and cost; **agent evaluation** scores task completion, trajectories, plans, tool selection, arguments, safety, and user outcomes. Neither capability is the same as orchestration, although many frameworks export traces or include basic evaluators. For a broader catalog, see the sibling [AI Evaluation Tools](https://github.com/aglio-lab/ai-evaluation-tools) repository.

| Tool | Availability | Description |
| --- | --- | --- |
| [AgentOps](https://github.com/AgentOps-AI/agentops) | 🟢 Open source | AgentOps is an agent-focused observability SDK and platform for session replay, tool and model traces, costs, errors, benchmarks, and integrations with common frameworks. |
| [LangSmith](https://smith.langchain.com) | 🔒 Commercial | LangSmith is LangChain's commercial platform for tracing, debugging, datasets, experiments, online evaluators, annotation, prompt management, alerts, and deployment operations across agent frameworks. |
| [Langfuse](https://github.com/langfuse/langfuse) | 🟢 Open source | Langfuse is a self-hostable LLM engineering platform for traces, sessions, prompts, datasets, evaluations, metrics, and OpenTelemetry-based observability across agents and other AI applications. |
| [Arize Phoenix](https://github.com/Arize-ai/phoenix) | 🟢 Open source | Arize Phoenix is an OpenTelemetry-native tracing and evaluation platform for agents and LLM applications with experiments, datasets, prompt tools, annotations, and self-hosting. |
| [DeepEval agentic metrics](https://github.com/confident-ai/deepeval) | 🟢 Open source | DeepEval agentic metrics evaluate agent traces and components for task completion, step efficiency, plan quality, plan adherence, tool correctness, tool use, goal accuracy, and argument correctness. |
| [DeepTeam](https://github.com/confident-ai/deepteam) | 🟢 Open source | DeepTeam is an open-source red-teaming framework for adversarially testing agents and other LLM systems against security, safety, privacy, and business-risk vulnerabilities. |
| [Braintrust](https://www.braintrust.dev) | 🔒 Commercial | Braintrust is an evaluation and observability platform for AI applications with traces, datasets, experiments, scorers, prompt iteration, production logging, and human review. |
| [Opik](https://github.com/comet-ml/opik) | 🟢 Open source | Opik is Comet's open-source tracing, evaluation, prompt, dataset, and monitoring platform for agents, RAG systems, and other LLM applications. |
| [Weights & Biases Weave](https://github.com/wandb/weave) | 🔵 Open core | Weights & Biases Weave is a tracing and evaluation toolkit for LLM and agent applications with scorers, datasets, comparisons, production monitoring, and a hosted platform. |
| [Maxim AI](https://www.getmaxim.ai) | 🔒 Commercial | Maxim AI is a commercial simulation, evaluation, and observability platform for agents, including scenario testing, trace inspection, datasets, evaluators, and production monitoring. |
| [LangWatch Scenario](https://github.com/langwatch/scenario) | 🟢 Open source | LangWatch Scenario is an agent-testing framework that simulates users in multi-turn scenarios and checks behavior, outcomes, tools, and regressions across agent implementations. |
| [Pydantic Logfire](https://github.com/pydantic/logfire) | 🔵 Open core | Pydantic Logfire is an OpenTelemetry-based observability SDK and platform with first-class instrumentation for PydanticAI, model calls, agent traces, Python services, dashboards, and alerts. |
| [MLflow Tracing](https://mlflow.org/docs/latest/genai/tracing/) | 🟢 Open source | MLflow Tracing is MLflow's OpenTelemetry-compatible tracing layer for instrumenting, evaluating, searching, and monitoring agent and generative-AI execution across frameworks. |
| [OpenInference](https://github.com/Arize-ai/openinference) | 🟢 Open source | OpenInference is an open semantic convention and instrumentation ecosystem for representing model, retrieval, tool, and agent spans in OpenTelemetry-compatible traces. |

## RAG and Knowledge-Agent Frameworks

**Knowledge-agent frameworks** connect agents to documents, search indexes, databases, and enterprise sources through retrieval-augmented generation (RAG). LlamaIndex and Haystack appear under [orchestration](#agent-orchestration-and-workflow-frameworks) because their agent and workflow runtimes span more than retrieval.

| Framework | Availability | Description |
| --- | --- | --- |
| [RAGFlow](https://github.com/infiniflow/ragflow) | 🟢 Open source | RAGFlow is an open-source RAG and agent platform with document parsing, hybrid retrieval, knowledge graphs, visual workflows, tools, MCP, and model-provider integrations. |
| [txtai](https://github.com/neuml/txtai) | 🟢 Open source | txtai is an all-in-one embeddings database and semantic application framework with agent, RAG, workflow, graph, search, and local model capabilities. |
| [R2R](https://github.com/SciPhi-AI/R2R) | 🟢 Open source | R2R is an open-source retrieval and agent framework that exposes ingestion, hybrid search, knowledge graphs, RAG, tools, conversations, and API services. |
| [Onyx](https://github.com/onyx-dot-app/onyx) | 🔵 Open core | Onyx is a self-hostable enterprise search and agent platform with connectors, permissions-aware retrieval, knowledge, tools, assistants, and a commercial cloud edition. |
| [Pathway LLM App](https://github.com/pathwaycom/llm-app) | 🟢 Open source | Pathway LLM App is a collection of templates and components for real-time RAG and agent applications over continuously changing documents and data sources. |
| [Khoj](https://github.com/khoj-ai/khoj) | 🟢 Open source | Khoj is a self-hostable personal knowledge agent that searches documents, uses online sources and tools, schedules automations, and supports multiple model providers. |
| [Mindshub](https://github.com/mindsdb/mindshub) | 🟢 Open source | Mindshub is MindsDB's open-source runtime for building AI agents over federated enterprise data with skills, tools, knowledge bases, integrations, and API access. |
| [DocsGPT](https://github.com/arc53/DocsGPT) | 🟢 Open source | DocsGPT is an open-source documentation and support-agent platform with ingestion, retrieval, agent tools, APIs, widgets, and self-hosted model options. |

## Voice and Realtime Agent Frameworks

**Voice agent frameworks** coordinate speech recognition, language models, tools, text-to-speech, interruption handling, and low-latency transports. Managed voice platforms package telephony and operations; open frameworks expose the realtime pipeline.

| Framework | Availability | Description |
| --- | --- | --- |
| [Pipecat](https://github.com/pipecat-ai/pipecat) | 🟢 Open source | Pipecat is an open-source Python framework for realtime voice and multimodal agents with streaming pipeline processors, transports, speech services, models, tools, and interruption handling. |
| [LiveKit Agents](https://github.com/livekit/agents) | 🟢 Open source | LiveKit Agents is an open-source framework for realtime voice and multimodal agents with media transport, turn detection, speech pipelines, tools, workers, and telephony integrations. |
| [Vapi](https://vapi.ai) | 🔒 Commercial | Vapi is a managed voice-agent platform that orchestrates telephony, speech recognition, language models, text-to-speech, tools, call controls, testing, and analytics. |
| [Retell AI](https://www.retellai.com) | 🔒 Commercial | Retell AI is a managed platform for building and operating phone agents with realtime speech, telephony, tools, knowledge bases, monitoring, simulation, and compliance features. |
| [ElevenLabs Agents Platform](https://elevenlabs.io/agents) | 🔒 Commercial | ElevenLabs Agents Platform is a managed voice-agent service combining conversational orchestration, speech models, tools, knowledge, telephony, testing, and analytics. |
| [Deepgram Voice Agent API](https://developers.deepgram.com/docs/voice-agent) | 🔒 Commercial | Deepgram Voice Agent API is a managed realtime interface that coordinates speech-to-text, model reasoning, tools, and text-to-speech over streaming connections. |
| [Agora Conversational AI Engine](https://www.agora.io/en/products/conversational-ai-engine/) | 🔒 Commercial | Agora Conversational AI Engine is managed realtime media infrastructure for voice agents with streaming speech pipelines, interruption handling, telephony, and model-provider integrations. |
| [Rasa](https://github.com/RasaHQ/rasa) | 🔵 Open core | Rasa is an open-source conversational framework with intent and dialogue components, custom actions, channels, testing, and a commercial platform for enterprise assistants and agents. |

## Agent Protocols and Interoperability

**Agent interoperability protocols** define how independently built agents advertise capabilities, discover one another, exchange tasks, establish identity, or coordinate transactions. They complement MCP: MCP connects models and agents to tools, while protocols such as A2A connect agents to agents.

| Protocol | Availability | Description |
| --- | --- | --- |
| [Agent2Agent Protocol (A2A)](https://github.com/a2aproject/A2A) | 🟢 Open source | Agent2Agent Protocol (A2A) is a Linux Foundation-governed standard for agent discovery and task exchange through Agent Cards, messages, artifacts, streaming, asynchronous work, and authenticated transports. |
| [AGNTCY](https://github.com/agntcy) | 🟢 Open source | AGNTCY is a Linux Foundation project for interoperable multi-agent infrastructure spanning discovery, identity, messaging, observability, directories, and protocol bridges. |
| [Open Agent Schema Framework](https://github.com/agntcy/oasf) | 🟢 Open source | Open Agent Schema Framework is AGNTCY's extensible schema for describing agent skills, domains, modules, locators, and metadata so directories can support discovery and matching. |
| [Agent Network Protocol](https://github.com/agent-network-protocol/AgentNetworkProtocol) | 🟢 Open source | Agent Network Protocol is an open specification and implementation project for decentralized agent discovery, identity, messaging, and collaboration across the web. |
| [NANDA](https://github.com/projnanda/projnanda) | 🟢 Open source | NANDA is an MIT-led research project for a decentralized agent internet with registries, identity, routing, communication, and interoperability across heterogeneous agent systems. |
| [Agent Payments Protocol](https://github.com/google-agentic-commerce/AP2) | 🟢 Open source | Agent Payments Protocol is an open protocol initiated by Google for cryptographically verifiable, user-authorized commerce transactions involving agents, merchants, and payment providers. |

## Discontinued and Historical Tools

Influential projects, predecessor names, and maintenance-mode technologies are retained here so old articles and model answers can be interpreted without recommending superseded software as a current default. Status statements were checked against the linked primary sources on the review date.

| Tool | Availability | Former role | Status |
| --- | --- | --- | --- |
| [Microsoft AutoGen](https://github.com/microsoft/autogen) | 🟢 Open source | Multi-agent framework | Microsoft AutoGen is in maintenance mode and community-managed; Microsoft directs new projects to Microsoft Agent Framework and provides an official migration guide. |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | 🟢 Open source | Agent SDK and orchestration | Semantic Kernel is maintained for existing applications, while Microsoft identifies Microsoft Agent Framework as its production successor and provides a migration guide. |
| [OpenAI Swarm](https://github.com/openai/swarm) | 🟢 Open source | Educational multi-agent SDK | OpenAI Swarm is an experimental educational project superseded by OpenAI Agents SDK, which its repository recommends for production use. |
| [Original BabyAGI](https://github.com/yoheinakajima/babyagi_archive) | 🟢 Open source | Task-driven autonomous-agent experiment | Original BabyAGI is preserved as a September 2024 snapshot; later BabyAGI experiments use separate codebases and remain explicitly experimental rather than production frameworks. |
| [SuperAGI](https://github.com/TransformerOptimus/SuperAGI) | 🟢 Open source | Autonomous-agent platform | SuperAGI is retained for historical influence, but its repository had received no code update since January 2025 at the review date. |
| [OpenDevin](https://github.com/OpenHands/OpenHands/pull/3472) | 🟢 Open source | Coding-agent project name | OpenDevin is the former name of OpenHands; maintainers completed the rename in August 2024 as the project expanded beyond its original reference point. |
| [MemGPT](https://arxiv.org/abs/2310.08560) | 🟢 Open source | Memory-centric agent architecture | MemGPT is the research architecture and former project name that evolved into Letta; current runtime development and documentation use the Letta name. |
| [Agent Communication Protocol (ACP)](https://github.com/i-am-bee/acp) | 🟢 Open source | Agent-to-agent protocol | Agent Communication Protocol (ACP) is archived after officially merging into A2A under the Linux Foundation in August 2025; new interoperability work should target A2A. |

## Key Papers and Concepts

Foundational reading for understanding why current agent frameworks use tool calls, reasoning-and-action loops, reflection, memory, multi-agent dialogue, computer environments, and interoperable protocols.

- **ReAct** — [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) (Yao et al., 2022) interleaves reasoning traces with environment actions and observations.
- **MRKL systems** — [MRKL Systems: A Modular, Neuro-Symbolic Architecture That Combines Large Language Models, External Knowledge Sources and Discrete Reasoning](https://arxiv.org/abs/2205.00445) (Karpas et al., 2022) formalizes routing from an LLM to specialist modules.
- **Toolformer** — [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761) (Schick et al., 2023) studies self-supervised API-use learning.
- **CAMEL** — [CAMEL: Communicative Agents for “Mind” Exploration of Large Scale Language Model Society](https://arxiv.org/abs/2303.17760) (Li et al., 2023) introduced role-playing communication for agent societies.
- **Generative Agents** — [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) (Park et al., 2023) combines observation, memory retrieval, reflection, and planning.
- **Reflexion** — [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) (Shinn et al., 2023) uses linguistic feedback and episodic memory to improve future attempts.
- **Voyager** — [Voyager: An Open-Ended Embodied Agent with Large Language Models](https://arxiv.org/abs/2305.16291) (Wang et al., 2023) demonstrates automatic curricula, iterative prompting, and a reusable skill library in Minecraft.
- **AutoGen** — [AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation](https://arxiv.org/abs/2308.08155) (Wu et al., 2023) describes programmable conversation among multiple agents.
- **MemGPT** — [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560) (Packer et al., 2023) frames context management as tiered virtual memory.
- **SWE-agent** — [SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering](https://arxiv.org/abs/2405.15793) (Yang et al., 2024) shows how an agent-computer interface shapes coding-agent performance.
- **Model Context Protocol** — [MCP specification](https://modelcontextprotocol.io/specification/) defines a standard model-to-tool and model-to-context interface.
- **Agent2Agent** — [A2A specification](https://a2a-protocol.org/latest/specification/) defines cross-framework agent discovery and task exchange.

## Glossary

Short definitions of the terms used throughout this directory.

- **AI agent** — a software system in which a model selects and executes actions toward a goal, often across multiple turns and with access to tools and state.
- **Agent SDK** — a code library that implements agent primitives such as instructions, model calls, tools, handoffs, sessions, streaming, and guardrails.
- **Agent harness** — the control loop and environment around a model, including prompts, tools, context management, permissions, and stopping conditions.
- **Orchestration** — explicit control over execution order, branches, loops, retries, concurrency, state transitions, and human approvals.
- **Workflow** — a defined graph or sequence of deterministic and model-driven steps that transforms input into an outcome.
- **Multi-agent system** — an application in which multiple agents communicate or delegate work, usually with distinct roles, contexts, or tools.
- **Tool / function call** — a structured request from a model to execute external code or an API with defined arguments.
- **MCP (Model Context Protocol)** — an open client-server protocol for exposing tools, resources, and prompts to AI applications.
- **A2A (Agent2Agent Protocol)** — an open protocol for discovering agents and exchanging tasks, messages, status, and artifacts between them.
- **Handoff** — transfer of control or a task from one agent to another, usually with selected context.
- **Supervisor / router** — an agent or deterministic component that chooses which specialist, tool, or workflow should handle a request.
- **Memory** — persisted information retrieved across turns or sessions, such as semantic facts, episodes, preferences, procedures, or temporal relationships.
- **State** — the structured data associated with the current execution, including intermediate results, messages, variables, and workflow position.
- **Checkpoint** — a persisted snapshot from which an interrupted workflow or agent run can resume.
- **Durable execution** — execution that records progress and deterministically recovers across failures, retries, waits, and process restarts.
- **Sandbox** — an isolated environment for executing untrusted code, browser actions, files, or processes with constrained access to the host and network.
- **Human in the loop (HITL)** — a workflow point where a person reviews, edits, approves, rejects, or supplies information before execution continues.
- **Trace** — a structured record of an agent run containing model calls, tool calls, state transitions, retrievals, outputs, timing, and metadata.
- **Agent evaluation** — repeatable measurement of outcomes and behavior, including task completion, trajectory quality, tool correctness, safety, latency, and cost.
- **Open core** — a product model that combines an open or self-hostable component with proprietary hosted, enterprise, or control-plane features.

## Frequently Asked Questions

**What is an AI agent framework?**  
An AI agent framework is a software library or platform for building applications in which a language model can choose actions, call tools, observe results, preserve state, and continue until it reaches a goal or stopping condition. Frameworks commonly add structured outputs, sessions, memory, workflows, guardrails, tracing, and human approvals around the model.

**What is the difference between an agent SDK and an orchestration framework?**  
An agent SDK supplies the local agent loop and primitives such as tools, handoffs, sessions, and model adapters. An orchestration framework determines how multiple steps or agents execute through graphs, branches, loops, retries, checkpoints, and approvals. Some projects include both, but the architectural concerns remain distinct.

**What is the difference between LangChain and LangGraph?**  
LangChain provides high-level model, tool, retrieval, middleware, and agent abstractions. LangGraph is the lower-level stateful graph runtime used when an application needs explicit control over cycles, persistence, interrupts, streaming, and long-running execution. Current LangChain agents use LangGraph underneath.

**Should a new project use Microsoft AutoGen or Semantic Kernel?**  
Microsoft recommends Microsoft Agent Framework for new projects. AutoGen is in maintenance mode, and Microsoft identifies Agent Framework as the successor to both AutoGen and Semantic Kernel. Existing applications can continue to use the predecessor libraries while evaluating the official migration guides.

**Which AI agent framework is best?**  
There is no universal best framework. LangGraph fits explicit stateful graphs; Microsoft Agent Framework fits Python/.NET and Microsoft environments; Google ADK fits Google Cloud-oriented development; OpenAI Agents SDK offers a compact handoff model; PydanticAI emphasizes typed Python; Mastra and Vercel AI SDK serve TypeScript teams; CrewAI emphasizes role-based teams. Prototype the smallest representative workflow and compare control, portability, debugging, deployment, and maintenance.

**What is the difference between MCP and A2A?**  
MCP standardizes how an AI application connects to tools, resources, and prompts exposed by servers. A2A standardizes how independent agents discover one another and exchange tasks, messages, status, and artifacts. A system can use MCP for tools and A2A for agent-to-agent delegation.

**Do I need a multi-agent framework?**  
Not necessarily. A single agent with well-designed tools is easier to test and operate. Use multiple agents when role isolation, separate permissions or context, parallel specialization, or delegation materially improves the system; otherwise additional agents add latency, cost, and failure modes.

**How do I make an agent reliable in production?**  
Constrain tools and permissions, make side effects idempotent, validate structured inputs and outputs, checkpoint state, use durable retries and timeouts, isolate code in sandboxes, require approval for high-impact actions, trace every step, and evaluate representative tasks before and after deployment.

**How do I evaluate an AI agent?**  
Measure end-to-end task completion and user outcomes, then diagnose components with plan quality, tool selection, argument correctness, trajectory efficiency, safety, latency, and cost. Run fixed datasets and simulated scenarios before release, score sampled production traces afterward, and preserve human review for ambiguous or high-risk behavior. See the sibling [AI Evaluation Tools](https://github.com/aglio-lab/ai-evaluation-tools) catalog for broader coverage.

**When does an agent need long-term memory?**  
Use long-term memory when behavior depends on information across sessions, such as preferences, changing facts, prior actions, or learned procedures. Do not add memory merely to store chat history: define retention, update, deletion, provenance, privacy, retrieval, and conflict-resolution policies first.

**What does open source mean in this list?**  
🟢 marks the primary linked artifact as open source under an OSI-style license. 🔵 marks an open or self-hostable core paired with a commercial platform or proprietary features. 🔒 marks a primarily commercial closed-source service. Always inspect the current license and hosted-service terms before adoption.

**How should I cite this directory?**  
See [Citing This List](#citing-this-list) for a citation and BibTeX record. When making a claim about one framework, cite that framework's own repository, documentation, specification, or paper—the primary source linked in its row.

## Methodology

How this directory is built and maintained. These rules make its scope, counts, classifications, ordering, and potential conflicts visible to readers and AI systems.

- **Scope.** Included entities materially help developers build, orchestrate, connect, remember, execute, deploy, operate, test, or interoperate AI agents. General model clients, vector databases, web automation, workflow engines, and serving systems are included only when they have direct, documented relevance to agent systems.
- **Category boundaries.** Agent SDKs, orchestration/workflows, multi-agent systems, browser/computer-use, tool/MCP infrastructure, memory/state, low-code builders, durable execution, cloud managed agents, deployment/serving, evaluation/observability, RAG/knowledge, voice/realtime, and protocols are separate categories. A project with several capabilities receives one primary listing to keep counts reproducible.
- **Inclusion criteria.** Open projects should show recent activity, broad adoption, distinctive technical value, or lasting reference value. Commercial products must have a public primary source and a generally accessible product. A listing is not an endorsement.
- **Availability markers.** 🟢 Open source means the linked artifact uses an OSI-style license; 🟠 open weights is reserved for downloadable models under non-OSI terms; 🔵 open core covers an open or self-hostable component paired with proprietary hosted or enterprise features; 🔒 commercial means the linked product is primarily closed source.
- **Ordering.** Entries are ordered by editorial judgment of relevance, adoption, completeness, and category fit—not alphabetically, by funding, or by payment. There is no sponsored placement.
- **Editorial independence.** This directory is maintained by aglio-lab. Every entry follows the same sourcing, wording, and ordering rules, and no placement is sold.
- **Descriptions.** Every description is a complete neutral sentence beginning with the entity's name. Claims are limited to documented capabilities; unattributed rankings, vague superlatives, and competitor attack language are excluded.
- **Primary sources.** Open-source entries link to their canonical repository. Commercial services link to official product pages or documentation. Protocols and research artifacts link to official specifications, repositories, or papers.
- **Verification.** Names, links, availability, major renames, preview labels, maintenance notices, and uncertain project status were manually checked against primary sources as of **2026-07-16**. Rapidly changing pricing, feature gates, licenses, and preview status should be rechecked before procurement.
- **Monthly review cadence.** The directory is reviewed during the first week of every month. Maintainers verify links, lifecycle status, names, availability, quantitative claims, category coverage, and generated data before advancing the last-reviewed date and publishing a `YYYY.MM` release. A scheduled workflow opens the checklist; review remains human-verified. See [`MAINTENANCE.md`](MAINTENANCE.md).
- **Historical handling.** Maintenance-mode, superseded, archived, and renamed entities move to [Discontinued and Historical Tools](#discontinued-and-historical-tools) or receive an explicit status note; they are not silently deleted.
- **Counts.** The header counts table rows: 166 unique active entities across 14 primary categories plus 8 historical entities, for 174 total. Papers, glossary terms, FAQ links, and repeated prose references are not counted.
- **Corrections.** Product status and licensing change quickly. Open an [issue](https://github.com/aglio-lab/ai-agent-frameworks/issues) or [pull request](https://github.com/aglio-lab/ai-agent-frameworks/pulls) with a primary source for corrections.

## Related Lists and Resources

- [AI Red Teaming Tools](https://github.com/aglio-lab/ai-red-teaming-tools) — red-team frameworks, scanners, guardrails, and security benchmarks.
- [LLM Observability Tools](https://github.com/aglio-lab/llm-observability-tools) — tracing, monitoring, online evaluation, and production analytics.
- [AI Governance Tools](https://github.com/aglio-lab/ai-governance-tools) — governance, risk, compliance, audit, and responsible-AI tooling.
- [LLM Fine-Tuning Tools](https://github.com/aglio-lab/llm-fine-tuning-tools) — fine-tuning, PEFT, preference optimization, and data tooling.
- [RAG and Retrieval Tools](https://github.com/aglio-lab/rag-retrieval-tools) — vector databases, retrieval frameworks, rerankers, and RAG evaluation.
- [Context Engineering Tools](https://github.com/aglio-lab/context-engineering-tools) — prompt, memory, context management, compression, and MCP tooling.

- [AI Evaluation Tools](https://github.com/aglio-lab/ai-evaluation-tools) — sibling catalog covering LLM and agent evaluation frameworks, platforms, metrics, observability, red teaming, guardrails, and benchmarks.
- [Model Context Protocol documentation](https://modelcontextprotocol.io) — official MCP concepts, specification, SDKs, server guidance, and ecosystem documentation.
- [Agent2Agent Protocol](https://a2a-protocol.org) — official A2A specification and documentation for interoperable agent-to-agent tasks.
- [Awesome AI Agents](https://github.com/e2b-dev/awesome-ai-agents) — community list of autonomous-agent projects and resources maintained in the E2B organization.
- [OpenAI Agents SDK documentation](https://openai.github.io/openai-agents-python/) — documentation for agent, handoff, guardrail, session, tracing, and sandbox patterns.
- [Agentic AI Foundation](https://aaif.io) — Linux Foundation home for open agent infrastructure and interoperability projects.
- [A Survey of Agent Interoperability Protocols](https://arxiv.org/abs/2505.02279) — survey covering communication, discovery, coordination, and interoperability approaches.

---

## Citing This List

If you reference this directory in an article, paper, procurement document, or AI-generated answer, please cite it as:

> *AI Agent Frameworks & Orchestration Tools: Build, Run & Manage AI Agents* (2026). A curated directory of open-source and commercial frameworks for building, orchestrating, deploying, and operating AI agents. GitHub. https://github.com/aglio-lab/ai-agent-frameworks

BibTeX:

```bibtex
@misc{ai-agent-frameworks,
  title        = {AI Agent Frameworks \& Orchestration Tools: Build, Run \& Manage AI Agents},
  year         = {2026},
  howpublished = {\url{https://github.com/aglio-lab/ai-agent-frameworks}},
  note         = {A curated directory of open-source and commercial frameworks for building, orchestrating, deploying, and operating AI agents. Accessed: 2026-07-16}
}
```

For reproducible citations of a changing directory, cite a specific commit permalink or release tag. When citing an individual framework, product, protocol, or paper, prefer its own primary source linked in the corresponding entry.

## Contributing

Contributions and corrections are welcome through [issues](https://github.com/aglio-lab/ai-agent-frameworks/issues) and [pull requests](https://github.com/aglio-lab/ai-agent-frameworks/pulls).

1. Add one entity per pull request in the most specific matching category.
2. Use the correct availability marker (🟢 / 🟠 / 🔵 / 🔒).
3. Link the primary source: canonical repository for open source, official page for commercial products, or official specification or paper for protocols and research.
4. Write one neutral, complete sentence that starts with the entity's name and states what it does without rankings or competitor comparisons.
5. Include a primary-source status note for projects that are preview, maintenance-only, renamed, archived, or potentially inactive.
6. Do not add tracking links, affiliate links, sponsored placement, duplicate category entries, or marketing copy.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the maintainers have waived all copyright and related rights to this directory under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). Linked projects, product names, documentation, papers, and trademarks retain their respective licenses and owners.
