# Mastra (mastra-ai)

Mastra is a TypeScript framework for building AI-powered applications and agents, built by the team behind Gatsby (Sam Bhagwat, Abhi Aiyer, Shane Thomas). The framework provides production-grade primitives for agents, workflows, RAG, tools, memory, evals, voice, and observability, and integrates with 40+ model providers through the Vercel AI SDK. The framework is Apache 2.0 licensed open source, with a hosted commercial offering (Mastra Cloud) for deployment, tracing, and team collaboration, and an enterprise self-hosted edition for regulated environments.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/mastra-ai/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Producing
- **Access:** Open Source
- **x-type:** opensource
- **Tier:** 2

## Tags

- Agents
- Artificial Intelligence
- Workflows
- RAG
- MCP
- Memory
- Evaluation
- LLM Observability
- TypeScript
- Voice
- Open Source

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Mastra Framework

TypeScript-first agentic stack distributed as the `@mastra/*` family of npm packages. Wires agents, workflows, memory, RAG, tools, MCP, evals, voice, and observability into a single Mastra instance that can be embedded in Next.js, Express, Hono, SvelteKit, Astro, Nest, Fastify, Koa, or stood up as a standalone server. Models are reached through the Vercel AI SDK so any of 40+ providers (OpenAI, Anthropic, Google, Bedrock, Groq, etc.) plug in through one interface. Apache 2.0 licensed.

- [Documentation](https://mastra.ai/docs)
- [Source Code](https://github.com/mastra-ai/mastra)
- [npm @mastra/core](https://www.npmjs.com/package/@mastra/core)

### Mastra Agents

Agents define behavior with a model, instructions, tools, memory, and processors, then expose `.generate()` and `.stream()` for typed text, object, and structured output generation. Supports multi-step tool calls, dynamic instructions, runtime context, scoped memory, and Vercel AI SDK v5 message format.

- [Documentation](https://mastra.ai/docs/agents/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/packages/core/src/agent)

### Mastra Workflows

Durable, graph-based pipelines composed from typed steps with branching, parallelism, loops, suspension, human-in-the-loop, and event triggers. Inputs and outputs are validated against Zod schemas and each run is persisted so workflows can be replayed, resumed, and observed.

- [Documentation](https://mastra.ai/docs/workflows/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/workflows)

### Mastra Memory

Conversation history, working memory, and semantic recall for agents, pluggable across PostgreSQL, LibSQL, Redis, Upstash, MongoDB, MS SQL, DynamoDB, Cloudflare D1, ClickHouse, Couchbase, and other backends. Vector recall integrates with PgVector, Pinecone, Chroma, Qdrant, Astra, Elasticsearch, OpenSearch, Turbopuffer, Vectorize, LanceDB, DuckDB, S3Vectors, and more.

- [Documentation](https://mastra.ai/docs/memory/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/packages/memory)

### Mastra RAG

Document loaders, chunkers, embedders (including FastEmbed local embeddings), rerankers, and retrieval helpers that compose with any Mastra vector store. Supports semantic, keyword, and hybrid retrieval, metadata filtering, and graph RAG patterns.

- [Documentation](https://mastra.ai/docs/rag/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/packages/rag)

### Mastra MCP

First-class Model Context Protocol support — an MCP client for connecting to any MCP server and exposing its tools to agents, plus an MCP server implementation for publishing your own agents, workflows, and tools as MCP-callable capabilities. Includes a docs MCP server and a registry-of-registries.

- [Documentation](https://mastra.ai/docs/mcp/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/packages/mcp)

### Mastra Evals

Built-in evaluation library with model-graded (LLM-as-judge), rule-based, and statistical metrics for measuring agent output quality, hallucination, faithfulness, relevance, bias, toxicity, and answer correctness. Evals run locally or against Mastra Cloud and emit traces alongside production runs.

- [Documentation](https://mastra.ai/docs/evals/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/packages/evals)

### Mastra Voice

Voice abstractions for speech-to-text, text-to-speech, and realtime voice agents with provider adapters for OpenAI (including Realtime API), ElevenLabs, Deepgram, Google, Google Gemini Live, Azure, AWS Nova Sonic, Gladia, Inworld, Murf, PlayAI, Sarvam, Speechify, ModelsLab, and xAI Realtime.

- [Documentation](https://mastra.ai/docs/voice/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/voice)

### Mastra Observability

OpenTelemetry-native tracing for agents, workflows, tools, and LLM calls with first-party exporters for Mastra Cloud, Langfuse, LangSmith, Braintrust, Arize, Arthur, Laminar, Datadog, Sentry, ClickHouse, and PostHog. AI SpanKind semantic conventions and an OTel bridge are supported out of the box.

- [Documentation](https://mastra.ai/docs/observability/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/observability)

### Mastra CLI

The `mastra` CLI scaffolds projects (`npm create mastra`), runs the local dev server with hot reload, opens the Studio playground, generates types, runs migrations on memory stores, deploys to Mastra Cloud, and runs evals.

- [Documentation](https://mastra.ai/docs/cli/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/packages/cli)
- [npm](https://www.npmjs.com/package/mastra)

### Mastra Client SDKs

Client-side SDKs that talk to a Mastra server from the browser, React applications, or any JavaScript runtime. Includes `@mastra/client-js` (universal JS client), `@mastra/react` (React hooks for agents, streaming, and workflows), and `@mastra/ai-sdk` (adapters for the Vercel AI SDK UI primitives).

- [Documentation](https://mastra.ai/docs/client-sdks/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/client-sdks)

### Mastra Deployers

Deployer packages that bundle a Mastra app for a target runtime. Built-in deployers cover Mastra Cloud, Cloudflare Workers, Vercel, and Netlify. Custom deployers can be written for any Node-compatible platform.

- [Documentation](https://mastra.ai/docs/deployment/overview)
- [Source Code](https://github.com/mastra-ai/mastra/tree/main/deployers)

## Common Properties

- [Website](https://mastra.ai)
- [Documentation](https://mastra.ai/docs)
- [GitHub](https://github.com/mastra-ai/mastra)
- [GitHub Org](https://github.com/mastra-ai)
- [Blog](https://mastra.ai/blog)
- [Releases / ChangeLog](https://github.com/mastra-ai/mastra/releases)
- [Pricing](https://mastra.ai/pricing)
- [npm @mastra Org](https://www.npmjs.com/org/mastra)
- [Examples](https://github.com/mastra-ai/mastra/tree/main/examples)
- [Templates](https://mastra.ai/templates)
- [Discord](https://discord.gg/BTYqqHKUrf)
- [X / Twitter](https://x.com/mastra_ai)
- [LinkedIn](https://www.linkedin.com/company/mastra-ai)
- [YouTube](https://www.youtube.com/@mastra-ai)
- [Y Combinator](https://www.ycombinator.com/companies/mastra)
- [Crunchbase](https://www.crunchbase.com/organization/mastra-44ba)
- [License — Apache 2.0 + Mastra Enterprise License](https://github.com/mastra-ai/mastra/blob/main/LICENSE.md)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
