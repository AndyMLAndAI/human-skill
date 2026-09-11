---
name: human
description: Rewrite or draft text so it reads as human-written, not AI-generated. Supports modes — academic (essays, papers, research writing), post (Reddit, Twitter/X, forums, LinkedIn, comments), normal (email, Slack/Teams, cover letters, everyday messages). Use whenever the user asks to "make this sound human", "de-AI this", "remove AI tone", humanize a draft, or write an essay/post/email/message and cares about it not reading as AI-generated. If mode isn't specified, infer it from context or ask.
---

# Human

Kill AI-tells. Calibrate to register. Never sound like a template.

Full research backing these rules: `research/human-writing-findings.md` in the project repo (only read if you need the "why" — the rules below are sufficient to execute).

## Step 1: Pick the mode

- **academic** → essays, papers, research writing, lit reviews → read `references/academic.md`
- **post** → Reddit, Twitter/X, forums, LinkedIn, comments, social → read `references/online.md`
- **normal** → email, Slack/Teams, cover letters, texts, everyday writing → read `references/normal.md`

If the user names a mode explicitly, use it. If not, infer from what's being written (essay = academic, tweet/comment = post, email/message = normal — this is the safe default). If genuinely ambiguous, ask one question.

Always apply the universal rules below regardless of mode. Then apply the mode-specific reference file on top.

## Universal Rules (apply in every mode)

### 1. Purge the AI lexicon
Delete these and their variants; replace with plain verbs/nouns:
- Verbs: delve, foster, navigate, leverage, elevate, unlock, embrace, showcase, illuminate, unravel, spearhead, bolster, transcend, underscore, empower, cultivate, orchestrate, harness
- Nouns: tapestry, testament, beacon, realm, landscape, paradigm, nexus, interplay, labyrinth, synergy, cornerstone, linchpin, conduit, bedrock
- Adjectives: multifaceted, paramount, pivotal, intricate, meticulous, profound, vibrant, robust, nuanced, transformative, commendable, bespoke, indelible, pervasive
- Adverbs: furthermore, moreover, additionally, fundamentally, seamlessly, inherently, indelibly, holistically, crucially, notably

### 2. Enforce burstiness (CV ≥ 0.65)
Never write three consecutive sentences of similar length. Pair a 4–7 word staccato sentence against a 30–50 word compound-complex one. Across any 300-word passage, sentence-length std-dev should be ≥ 9 words. Read it back — if it sounds metronomic, break it.

### 3. Cut throat-clearing and horizon-gazing
No "In today's fast-paced world," "When it comes to X," "It is important to note." Start on the claim, decision, or event. No "As we look to the horizon," "only time will tell," "X is poised to revolutionize Y." No summary paragraph that just restates what was already said — end on a concrete next step or stop.

### 4. Kill the tricolon reflex
Stop defaulting to "X, Y, and Z" lists/adjective triads. Use one strong point, two contrasting points, or four specific ones instead. When listing, mix concrete and abstract rather than keeping everything grammatically parallel.

### 5. Ration em-dashes and bold-colon spam
Max one em-dash per 500 words. No `**Label:** explanation` bullet format unless it's genuinely a reference table. Don't use a dash to tack a dramatic coda onto a sentence.

### 6. Kill antithetical parallelism
Delete "not only X, but also Y" / "not just X, but Y." State the thing directly.

### 7. Take a position
No forced both-sidesing or artificial consensus between sources/views. If two things conflict, say which one wins or exactly why the conflict is unresolved. Include the ugly parts — failed attempts, trade-offs, constraints — instead of smoothing everything into optimism.

### 8. Ground abstractions
Every technical or prestige term must carry actual weight — if deleting it doesn't change the meaning, delete it. Use numbers, dollar amounts, line counts, dates, physical details instead of vague grandiosity ("robust solution" → "cut latency from 400ms to 90ms").

## Self-check before returning output
- Read it back once. Does any sentence sound like it could open a corporate blog post? Cut it.
- Any word from the banned lexicon? Cut it.
- Three sentences in a row the same length? Break it.
- Ends with a "in conclusion" restate? Cut it.
