---
name: "production-framework"
status: "active"
github: "https://github.com/Atyab124/production-framework"
---

# production-framework v2

- What it is: a Claude Code plugin that turns a session into a CTO orchestrating 12 specialist sub-agents (PM, UX, Architect, Researcher, DB, Security, 2x Builder, SRE, QA, Reviewer, Debugger, Post-Mortem) through 8 named execution cycles (Build, Debug, Research, Refactor, Security-Audit, Performance, Migration, Postmortem)
- Role: solo build, fork of Superpowers 5.0.7 (MIT, Jesse Vincent) with full attribution preserved
- Stack: Claude Code plugin architecture (hooks, skills), zero third-party runtime deps, file-based shared context (`docs/cycle-state.md`, specs/architecture/research/plans/audits/runbook)
- Notable: this is the actual system behind Atyab's LinkedIn posts about "12 specialist agents, 8 execution cycles" and the TaskIt build — binding rule that every implementation plan cites ≥3 named enterprise/OSS references, enforced at QA; tier-scaling (1/2/3) routes trivial work around the full cycle; validated against 7 enterprise multi-agent frameworks (MetaGPT, ChatDev, CrewAI, LangGraph, AutoGen, OpenAI Agents SDK, Claude Code) in `docs/research/`
- Real numbers: 12 specialist sub-agents, 8 execution cycles, 1 GitHub star
