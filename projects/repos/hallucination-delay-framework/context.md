---
name: "Hallucination Delay Framework"
status: "experimental"
github: "https://github.com/Atyab124/LLM---NotePad"
---

# Hallucination Delay Framework

- What it is: an open-source Python framework that runs a primary chat LLM alongside a hallucination detector and a lightweight "flash" summarizer, auto-restarting the conversation from a clean, compact context the moment a hallucination is flagged
- Role: solo build
- Stack: Python, Strands agent orchestration, provider-agnostic (Ollama, OpenAI, Anthropic, Bedrock), Streamlit UI
- Notable: detection is grounded in cited research, not a guess — entropy-based token uncertainty (Nature 2024), metamorphic/self-consistency checks, an optional internal linear-probe method (MHAD, IJCAI 2024); ships its own test suite and documents its own limits plainly ("cannot eliminate all hallucinations... always implement additional verification layers")
- Real numbers: —
