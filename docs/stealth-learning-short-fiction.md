# Stealth Learning Short Fiction

This fork adds `stealth-learning-short-fiction`, a Story Skills workflow for turning exact English test/example sentences into short Japanese entertainment fiction.

## What it is for

Use it when you want students to read a genuinely enjoyable short story while repeatedly encountering the exact English sentences they need to remember.

The default reader experience is:

- story is primarily Japanese
- genre can vary freely: everyday life, romance, sports, horror, mystery, SF, fantasy, isekai, comedy, suspense, family, friendship, etc.
- exact target English sentences appear only at meaningful story moments
- each English sentence is followed immediately by its Japanese translation
- grammar explanation is not inserted into the fiction unless requested
- short length is preferred over overcomplicated plotting

## Core quality rule

A story must still work as entertainment after all English target blocks and translations are removed.

If it does not, rewrite it.

## Example request patterns

### One short story

> この試験範囲から3文使って、800〜1200字くらいの短いスポ根を作って。本文は基本日本語。対象英文は原文を一字一句変えずに入れて、その直下に日本語訳。勉強っぽくせず、読み物として面白くして。

### Let the skill choose the genre

> この例文10個を、自然に入るように3〜4本の短編へ分けて。ジャンルは毎回変えて。日常、ホラー、恋愛、スポ根などから一番相性のいいものを選んで。

### Horror

> このテスト文を使って短いホラーにして。説明は少なく、最後に嫌な余韻が残る感じ。英文の下には日本語訳をつけて。

### Full test-range anthology

> 添付した今回の試験範囲を全部確認して、対象英文を漏れなく抽出。1話に詰め込まず、2〜4文ずつ短編に分配して。作品ごとにジャンル・主人公・オチを変えて。本文には監査表を出さないで。

## Default length modes

- Micro: about 400–700 Japanese characters, 1–2 targets
- Standard: about 700–1,400 Japanese characters, 2–4 targets
- Extended: about 1,400–2,200 Japanese characters, 3–5 targets

These are defaults, not quotas. Story quality comes first.

## Target sentence policy

When the source is a supplied test, textbook, example bank, worksheet, PDF, DOCX, or image:

1. extract from the source instead of memory
2. preserve exact wording when the goal is test memorization
3. do not silently correct or paraphrase the target
4. place a Japanese translation directly below
5. keep source ambiguities/errors separate from the reader-facing fiction

## Full-range workflow

For an entire test range, the skill internally builds a coverage ledger, then groups sentences by semantic compatibility rather than simply by test order.

It varies genre and emotional structure across the anthology, then audits exact coverage after drafting.

See:

- `skills/stealth-learning-short-fiction/SKILL.md`
- `skills/stealth-learning-short-fiction/references/test-range-anthology.md`
- `skills/stealth-learning-short-fiction/references/target-sentence-embedding.md`
- `skills/stealth-learning-short-fiction/references/quality-gates.md`

## Reader-facing output

By default, the student should see only:

- title
- story
- embedded exact English target sentence
- Japanese translation immediately below each target

Coverage tables, grammar labels, target IDs, QA notes, and audit results stay hidden unless explicitly requested.
