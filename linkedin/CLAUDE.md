# linkedin/ — voice + profile knowledge, by person

Purpose: let an agent write or answer as a specific real person — either
*how* they'd phrase something (voice, from their actual posts) or *what*
they'd actually say on a topic (profile, from their real background) — never
a generic AI voice or a guessed opinion.

Repeating unit: a person. Each person gets a self-contained folder under
`people/` with up to two independent pillars, `voice/` and `profile/` —
nothing is shared between people, and neither pillar depends on the other.

## People

| Person | Voice | Profile | Entry point |
|---|---|---|---|
| Atyab | ✅ | — | `people/atyab/CLAUDE.md` |
| Aryan | ✅ | ✅ | `people/aryan/CLAUDE.md` |

## Adding a new person, or a new pillar for an existing one

1. Copy the relevant half of `_templates/person/` (`voice/`, `profile/`, or both) to `people/<name>/`.
2. **Voice**: drop raw posts into `corpus/posts.md`, then read them, sort by purpose,
   and write `categorization.md`, `dos-and-donts.md`, one `tone/<category>.md` per
   category — `people/atyab/voice/` is the worked example.
3. **Profile**: drop a raw source (e.g. LinkedIn export, transcribed to plain-text
   markdown — never a stored PDF/binary) into `corpus/`, then write a curated
   `profile.md` from it — `people/aryan/profile/` is the worked example.
4. Fill in `people/<name>/CLAUDE.md` from the template, add/update the row above.

## The one rule

Never mix two people, or mix voice and profile content, into one draft without
being deliberate about it — pick the person, then the pillar, first.
