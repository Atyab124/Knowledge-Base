---
name: "Arcade-Management (iFun City)"
status: "active"
github: "https://github.com/Atyab124/Arcade-Management"
---

# Arcade-Management — iFun City arcade management platform

- What it is: full-stack multi-tenant SaaS for running an arcade business — CRM, POS, party booking, WhatsApp marketing, loyalty rewards, machine maintenance, reporting
- Role: solo build, real product requirement doc + architecture plan in `docs/`
- Stack: Node.js 20 + Express + TypeScript + Prisma, PostgreSQL 16 with Row-Level Security for tenant isolation, Redis + BullMQ for queues/scheduling, React + Vite + Tailwind frontend, dedicated Google-Sheets sync worker, WhatsApp via Trengo
- Notable: real security/compliance posture — RLS-enforced tenant isolation, append-only audit log + consent events + points ledger, opt-in gated WhatsApp sends with quiet-hours windows, PII-preserving soft-delete on customer erasure; CI runs typecheck + tests on every push via GitHub Actions; fake clients (Trengo, Google Sheets) let the whole stack run in dev/CI with zero real credentials
- Real numbers: 65+ unit tests, 4 services running in parallel (API, web, sync-worker, scheduler)
