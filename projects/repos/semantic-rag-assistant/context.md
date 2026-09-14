---
name: "Semantic RAG Assistant"
status: "experimental"
github: "https://github.com/Atyab124/Semantic-RAG-Assistant"
---

# Semantic RAG Assistant (n8n + Ollama + Supabase)

- What it is: a local, private RAG assistant — semantic-chunks and embeds uploaded documents, answers questions against them
- Role: solo build
- Stack: n8n (workflow orchestration), Ollama (local LLM + embeddings, qwen2.5/deepseek-r1/nomic-embed-text), Supabase + pgvector (vector store), Docker Desktop
- Notable: fully local/open-source, no cloud API keys; honestly documents its own current limitations (manual-form input only, text-only documents, needs a real GPU — developed and verified running on a 4GB GTX 1650ti mobile)
- Real numbers: —
