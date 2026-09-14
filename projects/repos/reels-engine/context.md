---
name: "reel-factory (Reels-engine)"
status: "active"
github: "https://github.com/Atyab124/Reels-engine"
---

# reel-factory — talking-head video → Instagram Reel pipeline

- What it is: one raw talking-head recording goes in, one Reel-format edit (9:16, 30-60s, hook-first, captioned) comes out — the folder structure *is* the orchestration
- Role: solo build
- Stack: numbered pipeline stages (`stages/NN_*`), `_shared/` for rules that never change per video (voice/story, Reel format, cut rules), `runs/<slug>/` stamped from a template per video — no framework code, just files and one agent
- Notable: this is Atyab's own project built on the same Interpretable Context Methodology (ICM) that `_system/icm-architect/` and this very knowledge base use — folders carry sequencing, `runs/` carries state, two hard human checkpoints (message/hook approval, then cutlist approval) never get skipped. Real, working proof that the methodology holds up outside the knowledge-base context it was first applied in here.
- Real numbers: —
