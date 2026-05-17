# Umair Tufail

AI Engineer at Zapdeck.AI. M.Sc. Artificial Intelligence at BTU Cottbus.

I spend most of my time building agentic systems and making large language models cheaper to run in production. Lately I have been focused on multi agent orchestration, retrieval augmented generation pipelines, and quantization strategies that let you serve 8B models on consumer GPUs without losing much accuracy. I also care a lot about evaluation infrastructure and making sure models do not break silently in production.

I also won first and second place at Google and Meta/AMD hackathons, where I worked on low latency tool calling and Unsloth based optimization on AMD Instinct GPUs.

## Some things I have built

**Sovereign AI Router** (LangGraph, Pydantic AI, vLLM, PostgreSQL)

A multi agent routing system that keeps sensitive data local. It replaces PII with synthetic tokens stored in PostgreSQL, routes queries to local quantized models or EU hosted endpoints, and maintains full audit trails. Zero PII leakage in testing. Sub 100ms time to first token on local paths.

**Frugal LLM Factory** (Unsloth, PEFT, llama.cpp, FastAPI)

A fine tuning and quantization pipeline that trains domain adapted models on an A100 in under an hour, then compiles them down to GGUF for serving on an RTX 3060. Runs at 38 tokens per second with 86% lower inference cost compared to cloud A100s.

**Zero Trust MCP Gateway** (FastMCP, Starlette, OPA, PyTest)

A security hardened gateway for the Model Context Protocol. Fixes authorization bypasses in FastMCP custom routes and enforces JWT validation on every endpoint with negligible latency overhead.

**RAG Red Teaming Engine** (Ragas, Langfuse, Prometheus, CI/CD)

Automated evaluation pipeline that stress tests RAG systems with adversarial prompts. Intercepts 99% of jailbreak attempts and blocks deployments that fail safety thresholds.

There are a few more repos here covering vector search at scale, multimodal document parsing, and shadow deployment MLOps. Feel free to look around.

## Tools I use regularly

Python, PyTorch, LangGraph, Pydantic AI, vLLM, Unsloth, Qdrant, Redis, PostgreSQL, FastAPI, Docker, GitHub Actions, GitLab CI, AWS, and Lambda Labs.

## Links

[LinkedIn](https://linkedin.com/in/umairtufail)
