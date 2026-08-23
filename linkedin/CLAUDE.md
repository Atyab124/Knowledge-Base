# linkedin/ — voice knowledge bundle

What this repeats: nothing runs here. This is a model of how Atyab writes LinkedIn
posts, built for an agent to consult before drafting a new one.

## Load order for drafting a new post

| Step | Read | Why |
|---|---|---|
| 1 | `dos-and-donts.md` | Always — mechanics that hold across every category |
| 2 | `voice/<category>.md` | Exactly one — match the post's category (see step 3 if unsure) |
| 3 | `categorization.md` | Only if unsure which category applies, or auditing a past call |
| 4 | `corpus/posts.md` | Only if you need a raw, verbatim example beyond what's excerpted |

## Categories

sharing-knowledge · promoting-work · behind-the-scenes · hot-takes · networking-gratitude
— one file each in `voice/`, picked by purpose. Full definitions and per-post reasoning: `categorization.md`.

## The one rule

Never load all five `voice/*.md` files for one draft — pick the category first, then load only that file plus `dos-and-donts.md`.
