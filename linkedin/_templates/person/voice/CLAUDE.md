# {Person name} — voice (how they write)

What this repeats: nothing runs here. This is a model of how {Person name} writes
LinkedIn posts, built for an agent to consult before drafting a new one.

## Load order for drafting a new post

| Step | Read | Why |
|---|---|---|
| 1 | `../../../_shared/platform-conventions.md` | Always — mechanical facts true for every person, not just this one |
| 2 | `dos-and-donts.md` | Always — what's specific to {Person name} across every category |
| 3 | `tone/<category>.md` | Exactly one — match the post's category (see step 4 if unsure) |
| 4 | `categorization.md` | Only if unsure which category applies, or auditing a past call |
| 5 | `corpus/posts.md` | Only if you need a raw, verbatim example beyond what's excerpted |

## Categories

{Fill in once discovered from this person's own posts — categories are derived
per person, not copied from another person's set. See `../../../people/atyab/voice/`
for a worked example of the process and the shape it produces.}

## The one rule

Never load every `tone/*.md` file for one draft — pick the category first.
