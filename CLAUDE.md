# Knowledge base — root map

This repo is a growing set of self-contained pieces, each its own small workspace
with its own entry file. This file only routes; it never holds content.

## Pieces

| Piece | For | Entry point |
|---|---|---|
| `linkedin/` | Drafting/voice-matching LinkedIn posts | `linkedin/CLAUDE.md` |

## Adding a new piece

1. Give it its own top-level folder and its own `CLAUDE.md` — it must stand alone,
   no reads into another piece's internals.
2. Add one row to the table above. That's the only change this file ever needs.

## Not a piece

`_system/` holds tooling used to build/maintain this repo's own structure
(e.g. the icm-architect skill source) — not something an agent drafts from.
