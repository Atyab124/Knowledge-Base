# projects/ — Atyab's GitHub project context

Purpose: maintain durable context for every GitHub project Atyab has built,
so an agent can answer questions about his work, or draft content that
references it (e.g. a `linkedin/` post needing real project numbers), without
Atyab re-explaining the project from scratch each time.

Repeating unit: a project. Each gets its own folder under `repos/`, the same
internal shape — instantiated by copying `_templates/project/`, not built
from a blank page each time.

## Projects

17 projects catalogued from Atyab's public GitHub — full list, one line each,
with status: [_index/log.md](_index/log.md). Load one project's own
`repos/<slug>/context.md` for the task at hand; never load all 17 at once.

Standouts if the task is "what's most worth showing off": `production-framework`
(the actual system behind his LinkedIn posts about a CTO-agent build framework),
`arcade-management` (full multi-tenant SaaS, real security posture), `reels-engine`
(his own project built on this repo's own ICM methodology), `end-to-end-rag-pipeline`
(most complete RAG build — guardrails + eval harness).

**Known gap**: only public repos are represented (`gh` CLI isn't installed/
authenticated in this environment). If Atyab has private repos worth cataloguing,
their context needs to come from him directly, same as any project update.

## Adding a project

1. Copy `_templates/project/` to `repos/<slug>/`.
2. Fill in `context.md` — name, GitHub URL, one-line description, Atyab's
   role, tech stack, status, real numbers/metrics if any exist. Leave a
   section out entirely rather than filling it with a guess.
3. Add one row to the table above and one line to `_index/log.md`.
4. If a project needs deeper documentation later (architecture, decisions),
   add more files inside that project's own folder — the shape can grow.

## The one rule

Never load every project's `context.md` for one task — load the specific
project the task is actually about.
