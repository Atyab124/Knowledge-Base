---
category: all
layer: C
---

# LinkedIn Post Categories

Source: [`posts.md`](corpus/posts.md) — 14 posts. (The source file's own numbering repeats `9` and `12` once each; I've treated those as separate posts and labeled them `9a`/`9b` and `12a`/`12b` below so references are unambiguous.)

Five categories emerged from what's actually in the file — I started from your two examples (Sharing Knowledge, Promoting My Work) and built the rest from what the remaining posts actually do, not from a generic template.

## The five categories

| # | Category | Posts | What it's for |
|---|---|---|---|
| 1 | **Sharing Knowledge** | 4, 6, 10, 11 | Teach one concrete, generalizable lesson pulled from real hands-on work |
| 2 | **Promoting My Work** | 1, 3, 7, 9a | Prove something real got built/shipped; credibility for clients, collaborators, recruiters |
| 3 | **Behind-the-Scenes** | 2 | Raw, low-effort process update — building in public, no polish, no pitch |
| 4 | **Opinions & Hot Takes** | 5, 8, 9b | Provocative stance on AI/work/business, built to be quoted or argued with |
| 5 | **Networking & Relationship Capital** | 12a, 12b | Gratitude / access / who you're learning from — credibility by association |

Voice guide for each: [voice/sharing-knowledge.md](voice/sharing-knowledge.md) · [voice/promoting-work.md](voice/promoting-work.md) · [voice/behind-the-scenes.md](voice/behind-the-scenes.md) · [voice/hot-takes.md](voice/hot-takes.md) · [voice/networking-gratitude.md](voice/networking-gratitude.md)

## Post-by-post

1. **"Everyone is asking whether AI agents can write error free production code."** → **Promoting My Work** (primary), Sharing Knowledge (secondary). The TaskIt case study — heaviest data density in the file (97% vs 14%, 150 users, 73 projects). Structured like a technical teardown, but its job is proof-of-work, not tips.
2. **"I wanted to see if Claude Code could really run unsupervised for 18 hours..."** → **Behind-the-Scenes**. The only clear example of this register in the file — see the caveat in [voice/behind-the-scenes.md](voice/behind-the-scenes.md).
3. **"Claude Ultra Code"** → **Promoting My Work**. Competitive positioning — draws the boundary between your framework and a competing tool.
4. **"What do you think?"** → **Sharing Knowledge**. A single tactical prompting trick, tightly told.
5. **"This is exactly it."** → **Opinions & Hot Takes**. Commentary on AI-and-jobs sentiment, no proof-of-work attached.
6. **"LLMs are like women...."** → **Sharing Knowledge** (primary), Opinions (secondary, for the edgy opener). The substance is a real lesson (context drift → restart sessions); the opener is a hot-take-style hook.
7. **"Claude Code is sh*t."** → **Promoting My Work**. Diagnoses a real limitation, then pivots straight into the framework pitch and two shipped products.
8. **"AI is too stupid to replace humans."** → **Opinions & Hot Takes**. Hammer/carpenter analogy, no specific proof attached — a stance, not a case study.
9. a. **"Most AI agent demos are sh*t."** → **Promoting My Work**. Same shape as #7: knock the industry, then show two real (unreleased) builds plus a named coworker as social proof.
   b. **"Hot take: I dont think anyone wants to be rich."** → **Opinions & Hot Takes** (primary), Networking (secondary). Opens as a stated hot take and closes on a general philosophy; the body happens to be an extended tribute to one person (Ajay).
10. **"Can AI be too smart?"** → **Sharing Knowledge**. Full case study of a failed approach and the general principle extracted from it — the cleanest "lesson from failure" post in the set.
11. **"If you walk into an AI interview without using AI…"** → **Sharing Knowledge**. Interview narrative used as a vehicle for a concrete tools list and one general skill claim (adaptive learning).
12. a. **"Yesterday taught me that you grow fastest..."** → **Networking & Relationship Capital**. Event recap, six people named with a one-line credential/insight each.
    b. **"I Think I Finally Get It."** → **Networking & Relationship Capital**. The philosophy version of 12a with no specific event attached.

## Judgment calls worth flagging

- **Category 3 has one example.** It's tonally distinct enough from Promoting My Work (much rawer, ends on an unrelated car photo, no pitch) that I kept it separate rather than folding it in — but treat its voice doc as a first draft until there's more source material to confirm the pattern.
- **9b sits between Opinions and Networking.** Filed under Opinions because it opens with an explicit stance ("Hot take") and closes on a portable principle — the same shape as 5 and 8 — but it functions partly as a tribute post. If you think of it as networking first, move it and use 12a/12b's voice doc instead.
- **Two numbering typos in the source file**: `9` and `12` each label two different posts. I didn't touch your original file — just flagging why the labels above use `9a/9b` and `12a/12b`.

Let me know if any of these calls should flip, or if you see a category I missed entirely.
