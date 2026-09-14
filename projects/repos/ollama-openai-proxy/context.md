---
name: "Ollama OpenAI-Compatible Proxy"
status: "shipped"
github: "https://github.com/Atyab124/Ollama_proxy-for-open-AI-api-usage"
---

# Ollama OpenAI-Compatible Proxy

- What it is: a lightweight Flask proxy that makes a local Ollama server look like a remote, OpenAI-compatible API (chat completions + embeddings)
- Role: solo build
- Stack: Python + Flask, ngrok for tunneling, streaming response support
- Notable: drop-in replacement lets OpenAI-only clients (GraphRAG, LangChain, LlamaIndex) run against local open-source models instead — maps `/v1/chat/completions` and `/v1/embeddings` to Ollama's native API and reformats responses to match OpenAI's schema
- Real numbers: —
