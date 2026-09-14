# Aryan — voice (how he writes)

What this repeats: nothing runs here. This is a model of how Aryan writes
LinkedIn posts, built for an agent to consult before drafting a new one. Built
independently from Atyab's — the categories, register, and rules below don't
carry over from his file at all.

## Load order for drafting a new post

| Step | Read | Why |
|---|---|---|
| 1 | `../../../_shared/platform-conventions.md` | Always — mechanical facts true for every person, not just Aryan |
| 2 | `dos-and-donts.md` | Always — what's specific to Aryan across every category |
| 3 | `tone/<category>.md` | Exactly one — match the post's category (see step 4 if unsure) |
| 4 | `categorization.md` | Only if unsure which category applies, or auditing a past call |
| 5 | `corpus/posts.md` | Only if you need a raw, verbatim example beyond what's excerpted |

## Categories

webinar-pitch · webinar-social-proof · system-breakdown · product-case-study · technical-opinion
— one file each in `tone/`, picked by purpose. Full definitions and per-post reasoning: `categorization.md`.

Note the skew: 4 of 5 categories end in an explicit CTA. Only `technical-opinion`
carries none — treat that absence as a real signal of category, not an omission.

## The one rule

Never load every `tone/*.md` file for one draft — pick the category first, then load only that file plus `dos-and-donts.md`.
