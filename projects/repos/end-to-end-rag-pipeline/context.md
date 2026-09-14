---
name: "RAG Q&A System"
status: "active"
github: "https://github.com/Atyab124/End-to-End-RAG-Pipeline"
---

# End-to-End RAG Pipeline

- What it is: a fully local, production-shaped RAG system that answers questions over the user's own documents (.md/.txt/.pdf/.docx), with safety guardrails and a built-in evaluation harness
- Role: solo build
- Stack: Python, Ollama (local LLM + embeddings), FAISS (vector index), SQLite (metadata/persistence), Streamlit + CLI interfaces
- Notable: the most complete RAG build in the portfolio — prompt-injection detection, PII redaction, and grounding validation before an answer ships; every answer attributed back to source chunks; ships its own evaluation harness (Exact Match, F1, semantic similarity, retrieval success, grounding score) and a real-time observability module (query latency, memory/CPU, long-term reporting)
- Real numbers: —
