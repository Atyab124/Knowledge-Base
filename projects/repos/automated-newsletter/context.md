---
name: "Automated Newsletter Generator"
status: "active"
github: "https://github.com/Atyab124/Automated-Newsletter"
---

# Automated Newsletter Generator

- What it is: a Python system that scrapes multiple sources, builds verified fact sheets, and generates newsletters written in the user's own voice, on a schedule
- Role: solo build
- Stack: Python, Streamlit UI, SQLite, Ollama for generation, Playwright MCP for scraping, arXiv + Semantic Scholar APIs for research papers
- Notable: learns writing style from uploaded samples rather than a fixed prompt; newsletter generation is constrained to only use facts from the generated fact sheet (explicit anti-hallucination design, every claim sourced) — this fact-sheet-gate pattern shows up again later in the more mature End-to-End RAG Pipeline's grounding validation
- Real numbers: —
