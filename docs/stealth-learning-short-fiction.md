# Stealth Learning Short Fiction

This fork adds `stealth-learning-short-fiction`, a Story Skills workflow for turning exact English test/example sentences into **one-shot Japanese short-short fiction**.

## What it is for

Use it when you want students to read a genuinely enjoyable story while repeatedly encountering the exact English sentences they need to remember.

The default reader experience is:

- one complete standalone story
- about **2,000–3,500 Japanese characters**
- **5 exact source-grounded English targets per story** when at least five are available
- story is primarily Japanese
- genre can vary freely: comedy, everyday life, romance, sports, horror, mystery, SF, fantasy, isekai, suspense, family, friendship, etc.
- target English sentences appear at meaningful story moments
- each target is followed immediately by its Japanese translation
- grammar explanation is not inserted into the fiction unless requested
- the story has a real hook, escalation, turn, and ending rather than serving as a chain of example sentences

## Core quality rule

Delete all five English target blocks and their translations.

If the remaining Japanese story is not still worth reading, rewrite it.

A second rule is equally important:

> Five targets must belong to one story. Do not create five mini-scenes just to place five sentences.

## Integrated short-short craft

This fork now incorporates adapted craft ideas from public MIT-licensed fiction skills, especially:

- jwynia/agent-skills `flash-fiction`
- jwynia/agent-skills `story-analysis`

The integrated workflow checks:

- compact scope rather than a miniature novel
- opening hook
- paragraph economy
- character compression
- subtext
- setting that affects events
- escalation
- a meaningful turn
- emotional architecture
- opening/ending relationship
- genre promise
- twist dependency
- vignette trap
- resolution and aftertaste
- five-target cohesion
- student reader engagement

The upstream skills are inspiration/reference material; this fork adapts the ideas to five-target Japanese educational fiction rather than simply copying their workflow unchanged.

## Example request patterns

### One comedy short-short

> 暗唱例文から5文使って、2,000〜3,500字くらいの1話完結コメディを作って。本文は基本日本語。英文は原文のまま、その直下に日本語訳。5文を順番に消化する感じにはせず、普通に読み物として笑える話にして。

### Let the skill choose the genre

> この試験範囲から5文選んで、1話完結のショートショートを作って。ジャンルは例文との相性で決めて。英語を消しても読み物として成立すること。

### Horror

> この範囲から5文使って、長めのショートショートのホラーにして。2,000〜3,500字。説明しすぎず、途中から違和感が増えて、最後に嫌な余韻が残る感じ。

### Full test-range anthology

> 添付した試験範囲を全部確認して、5文ずつ1話完結の短編集にして。作品ごとにジャンル・主人公・人間関係・オチを変えて。最後に4文余ったら、既出1文を復習として再登場させて1話5文にして。本文には監査表を出さないで。

## Five-target policy

When at least five authoritative source targets are available, a standard story uses exactly five.

Each target must have:

- an exact source string
- its correct/approved Japanese translation
- a distinct story function
- a distinct memory anchor

If fewer than five source targets exist, use all available targets and do not invent another.

For a full-range anthology, if the final batch contains fewer than five unused targets, fill the remaining slots with previously covered source targets as deliberate spaced review.

## Target sentence policy

When the source is a supplied test, textbook, example bank, worksheet, PDF, DOCX, or image:

1. extract from the source instead of memory
2. preserve exact wording when the goal is test memorization
3. do not silently correct or paraphrase the target
4. place a Japanese translation directly below
5. protect target blocks from natural-Japanese or textlint rewriting
6. keep source ambiguities/errors separate from reader-facing fiction

## Mandatory quality passes

Every story goes through:

1. target/source verification
2. entertainment premise design
3. character voice cards
4. short-short blueprint + five-target placement map
5. Japanese-first drafting
6. exact target insertion
7. short-short craft pass
8. story analysis pass
9. natural Japanese fiction pass
10. character voice/dialogue pass
11. AI-writing detector/textlint review when available
12. final five-target/source audit

## Full-range workflow

For an entire test range, the skill builds a hidden coverage ledger, groups sentences by semantic compatibility rather than textbook order, and produces varied one-shot stories.

Coverage tracking distinguishes:

- new target coverage
- deliberate review reuse

This keeps every story at five targets without pretending repeated sentences are new coverage.

See:

- `skills/stealth-learning-short-fiction/SKILL.md`
- `skills/stealth-learning-short-fiction/references/short-short-fiction-craft.md`
- `skills/stealth-learning-short-fiction/references/story-analysis-pass.md`
- `skills/stealth-learning-short-fiction/references/test-range-anthology.md`
- `skills/stealth-learning-short-fiction/references/character-voice-dialogue.md`
- `skills/stealth-learning-short-fiction/references/natural-japanese-fiction-pass.md`
- `skills/stealth-learning-short-fiction/references/ai-writing-textlint-gate.md`
- `skills/stealth-learning-short-fiction/references/quality-gates.md`

## Reader-facing output

By default, the student sees only:

- title
- story
- five embedded exact English target sentences
- Japanese translation immediately below each target

Coverage tables, grammar labels, target IDs, QA notes, and audit results stay hidden unless explicitly requested.
