---
name: stealth-learning-short-fiction
description: Use this skill when the user wants an engaging Japanese short-short story, light-novel-style reading passage, genre fiction, or narrative learning material that naturally embeds exact target English sentences and their Japanese translations for memorization or test preparation. Suitable for comedy, slice-of-life, romance, sports, horror, mystery, suspense, SF, fantasy, isekai, family, friendship, and other genres. By default, the user's selected source range becomes one complete story, and story length scales with the number and narrative density of source-grounded target sentences.
---

# Stealth Learning Short Fiction

## Purpose

Create **Japanese fiction that is genuinely worth reading**, while embedding exact English test/example sentences so that scenes, emotions, and story events become memory anchors.

The primary product is fiction. Learning is hidden underneath the story design.

This skill is not limited to fantasy, isekai, school stories, romance, or any single genre.

## Default Unit: User-Selected Range = One Story

Unless the user explicitly asks for multiple stories, an anthology, separate genres, or separate outputs:

- treat the exact lesson/test/page/range selected by the user as **one story unit**
- include **all source-grounded target sentences in that selected range**
- do **not** automatically split the range into batches of five or any other fixed count
- do **not** invent review targets merely to reach a target count
- keep one central protagonist or one central relationship/problem unless the genre strongly requires otherwise
- allow multiple scenes inside the same story when needed, but preserve continuity of character, conflict, and emotional investment
- target order follows story logic rather than textbook order unless source order is naturally better
- every target English sentence is immediately followed by its Japanese translation
- the story remains overwhelmingly Japanese

The user's selected range is the primary boundary. Target count is not.

### Default Length Scaling

Use the following as a planning range, not a quota:

| Number of target sentences | Approximate Japanese story length |
|---|---:|
| 1–2 | 800–1,400 characters |
| 3–4 | 1,400–2,200 characters |
| 5–6 | 2,200–3,200 characters |
| 7–9 | 3,200–4,500 characters |
| 10–12 | 4,500–6,000 characters |
| 13+ | scale upward as needed; do not split solely because of count |

A useful rough heuristic is **500–700 base characters + roughly 400–500 characters per target sentence**, but story needs override arithmetic.

Length must also reflect semantic density:

- simple factual/routine targets may need less space
- regret, conflict, relationship change, mystery, suspense, or emotional targets may need more space
- do not pad to hit a number
- do not compress so aggressively that the reader cannot become emotionally invested

If a large selected range would become unwieldy, first use internal scene or act breaks within the same story. Split into separate stories only when the user requests it or when the selected source itself clearly consists of separate requested units.

## Core Principle

> Story first. User-selected target set second. Explanation last.

A finished story must pass all of these tests:

1. **Story-First Test** — remove all English blocks and translations; the Japanese story still works as fiction.
2. **Target-Set Cohesion Test** — the selected targets belong to one coherent narrative rather than a chain of stitched examples.
3. **Emotional-Investment Test** — the reader has enough time with the protagonist, relationship, problem, or mystery to care what happens next.
4. **Memory-Anchor Test** — each target has a specific memorable scene, action, joke, fear, relationship beat, image, or revelation.
5. **Short-Fiction Craft Test** — the story has an appropriate scope, strong opening, escalation, a meaningful turn, and an ending that rewards the setup.
6. **Native-Japanese Test** — the Japanese reads like natural contemporary fiction, not translated or prompt-generated prose.
7. **Character-Voice Test** — dialogue belongs to the specific speaker/listener relationship and emotional state.
8. **AI-Writing Review** — AI-like wording/structure detectors are used as warnings when available, followed by contextual judgment rather than blind replacement.

If any test fails, revise before delivery.

## Source Grounding

When the user supplies a textbook, test, example bank, worksheet, PDF, DOCX, image, or other source:

- treat supplied material as authoritative for target sentences and scope
- extract target English exactly from the source
- do not silently modernize, simplify, paraphrase, correct, or replace a target sentence
- if a source sentence appears erroneous or ambiguous, preserve it for exact-test practice and flag the concern separately rather than silently changing it
- use the source's Japanese translation when faithful reproduction is requested
- if natural translation is allowed, do not change the target meaning
- do not invent grammar rules or test coverage unsupported by the source
- never reconstruct source sentences from memory when the source is available

Maintain an internal target-sentence ledger before drafting.

For a lesson/test/range with multiple targets, also use `references/test-range-anthology.md`; despite the historical filename, its default behavior is now **single-story range planning**, not automatic anthology splitting.

## Reader-Facing Target Format

The story remains primarily Japanese. At a meaningful moment, insert:

**She might have sent the message to the wrong person.**  
彼女は間違った人にメッセージを送ってしまったかもしれない。

Then return immediately to the story.

The target block does **not** have to exist literally inside the fictional world. It may be a reader-facing learning insert attached to the matching moment.

Use a target as actual dialogue, chat, article text, sign, announcement, or narration only when the setting naturally justifies that English.

Never make Japanese characters suddenly speak/type English merely because the target must appear.

## Workflow

### 1. Lock the selected target set

Before inventing the plot, record every source target in the user-selected range:

- exact English
- exact/approved Japanese translation
- source location
- grammar/meaning supported by the source
- semantic situation
- whether it is new coverage or deliberate review only when review was actually requested

Do not draft until the strings are stable.

### 2. Set the story length from target count and story needs

Use the length-scaling table as a starting point.

Then adjust for:

- number of required targets
- how different their semantic situations are
- how much setup is needed to make them belong to one incident or relationship
- genre pacing
- emotional depth
- number of scenes needed

Never split merely because there are more than five targets.

### 3. Create the entertainment promise first

Ignore English for a moment and state internally why a student would continue reading.

Specify:

- genre
- intended reader emotion
- protagonist's immediate want
- obstacle/uncertainty
- what escalates
- what changes at the turn
- what kind of aftertaste the ending should leave

If the premise is not interesting in one or two Japanese sentences without mentioning grammar, replace it.

Examples of good promises:

- a harmless lie becomes increasingly difficult to correct
- an ordinary school room starts obeying one impossible rule
- two people want opposite things from the same conversation
- a player planning to quit discovers something that changes the decision
- one ordinary detail contradicts everyone's version of an event

### 4. Lock character voice before dialogue

If the story contains dialogue, read `references/character-voice-dialogue.md`.

Create an internal voice card for each speaker:

- age / school year / life stage
- personality
- relationship to the listener
- social distance / status
- directness
- talkativeness
- teasing style
- politeness
- address terms
- typical sentence shape
- emotional-state changes
- phrases this person would rarely or never use

Do not use age/gender stereotypes as a voice generator.

### 5. Build the story blueprint

Read `references/short-short-fiction-craft.md`.

Default story architecture:

1. Hook
2. Setup / immediate want
3. Escalation
4. Meaningful turn
5. Consequence
6. Aftertaste

Then create an internal target-placement map with one row per target:

| Target | Story job | Approximate region | Memory anchor |
|---|---|---|---|
| T1 | establish / complicate / reveal / decide / pay off | opening / middle / late | specific cue |

Rules:

- every target needs a real narrative job
- avoid back-to-back target blocks unless the scene genuinely requires it
- do not create one separate incident per target
- target order follows story logic, not source order, unless both happen to match
- no target may appear only because it was unused
- if several targets seem incompatible, redesign the central incident, relationship, setting, or timeline before considering a split

### 6. Draft the Japanese story first

Draft the actual fiction primarily in Japanese, using placeholders for target moments if useful.

Follow:

- `references/short-short-fiction-craft.md`
- `skills/chapter-writing/references/writing-guidelines.md`
- `references/japanese-prose-style.md`
- `references/character-voice-dialogue.md` for dialogue scenes

Do not manufacture a light-novel voice through:

- fragment chains
- exaggerated self-commentary
- constant witty metaphors
- anime-like perfect banter
- decorative punctuation
- quotable lines in every paragraph

Believable Japanese comes first.

### 7. Embed all selected targets surgically

Insert each exact target only where the scene already supports its meaning.

Immediately place the Japanese translation below it.

Do not:

- paraphrase exact targets
- split target sentences unless explicitly requested
- force targets into spoken dialogue
- put several targets consecutively like a list
- pause to explain grammar
- invent an unnatural situation solely to justify English

If any target does not fit, redesign the plot earlier. Do not append leftover targets near the ending as homework.

### 8. Run the Short-Fiction Craft Pass

Use `references/short-short-fiction-craft.md` again after drafting.

Specifically check:

- opening hook
- appropriate scope for the selected target count
- paragraph economy
- character compression without emotional thinness
- subtext
- setting that affects events
- escalation
- meaningful turn
- opening/ending relationship
- genre promise
- twist dependency
- vignette trap
- miniature-novel problem
- whether the reader has enough uninterrupted time with the same people/problem to care

Revise structure before polishing sentences.

### 9. Run the Story Analysis Pass

Read `references/story-analysis-pass.md`.

Audit:

- narrative foundation
- protagonist's concrete stake/want
- character behavior and relationships
- setting function
- decisive turn
- scene purpose
- emotional architecture
- information flow
- subtext
- resolution/aftertaste
- target-set cohesion
- reader engagement

Fix macro problems before micro prose.

### 10. Run the mandatory Natural Japanese + Character Voice Pass

Read both in full:

- `references/natural-japanese-fiction-pass.md`
- `references/character-voice-dialogue.md`

Repair:

- translationese / English-shaped syntax
- pseudo-light-novel fragment chains
- repeated subject marking
- mechanical sentence endings
- decorative punctuation
- explanatory inner monologue
- generic AI metaphors
- dialogue that sounds written rather than spoken
- dialogue inconsistent with age/relationship/personality/status/emotion
- interchangeable character lines
- unnaturally polished banter
- redundant emotional explanation

Run:

- mental read-aloud test
- speaker substitution test
- listener/register test

### 11. Run the AI-Writing Detector Review

Read `references/ai-writing-textlint-gate.md`.

When available, use:

- `p1ass/textlint-rule-preset-ai-words-ja`
- `textlint-ja/textlint-rule-preset-ai-writing`

Protect exact English targets and required Japanese translations before linting.

Classify findings as:

- KEEP
- REVIEW
- REWRITE

Do not chase zero warnings or mechanically replace words.

### 12. Run learning revision

Verify:

- every source-grounded target in the user's selected range appears
- every target matches the source exactly
- every target has the correct Japanese translation directly below it
- each target has a distinct memory anchor
- surrounding Japanese does not distort target meaning
- no grammar lecture leaked into the story
- no target was invented to satisfy a count
- the selected range was not silently split because of target count

Do not let this pass reintroduce unnatural Japanese.

### 13. Run final quality gates

Use `references/quality-gates.md`.

Automatic failure patterns include:

- worksheet wearing a costume
- grammar teacher disguised as a character
- example sentences connected by filler
- one mini-scene per target
- automatic five-sentence batching
- needless protagonist/world resets within one requested range
- overcomplicated plot built only to justify targets
- technically grammatical but AI-like Japanese
- generic teenager dialogue
- story that is boring until a final twist
- beautiful atmosphere with no narrative movement
- miniature novel compressed into summary

## Genre Selection

If the user specifies a genre, follow it.

If unspecified, choose from target semantics. For a single selected range, choose one coherent genre or a compatible blend rather than changing genre every few targets.

Possible genres include:

- comedy / school comedy
- slice-of-life
- romance / romantic comedy
- sports
- horror
- mystery
- suspense
- SF
- fantasy
- isekai
- friendship
- family drama
- workplace
- adventure
- bittersweet drama

Use `references/genre-presets.md` as guidance, not rigid templates.

## Multiple-Story / Anthology Mode

Use multiple one-shot stories only when the user explicitly requests multiple stories, an anthology, genre variation, separate units, or clearly separate outputs.

When multiple stories are requested:

- divide by the user's requested units first, not by a fixed target count
- do not standardize automatically on five targets per story
- scale each story's length to the targets assigned to that story
- vary genre, protagonist, relationship, conflict, ending shape, POV, and rhythm when variation is desired
- never invent a target to equalize story counts
- track coverage internally so no required target is dropped

## Reader-Facing Output

By default, show only:

1. title
2. story
3. all embedded target English blocks with their Japanese translations as part of the story flow

Do not expose:

- target IDs
- grammar labels
- coverage tables
- audit results
- QA notes

unless the user asks.

## Reference Files

- `references/short-short-fiction-craft.md` — integrated short-fiction craft: compression, hook, escalation, turn, subtext, frame, variable-target architecture
- `references/story-analysis-pass.md` — post-draft story diagnostic: foundation, characters, setting, turn, emotional architecture, resolution, reader engagement
- `references/short-story-craft.md` — earlier compact-story guidance
- `references/genre-presets.md` — genre-specific reader promises and pressures
- `references/target-sentence-embedding.md` — exact target preservation and insertion
- `references/japanese-prose-style.md` — natural Japanese narrative voice
- `references/natural-japanese-fiction-pass.md` — mandatory Japanese revision
- `references/character-voice-dialogue.md` — mandatory character-specific dialogue system
- `references/ai-writing-textlint-gate.md` — AI-like vocabulary/structure detector workflow
- `references/memory-design.md` — scene-based recall anchors
- `references/test-range-anthology.md` — selected-range single-story planning, optional anthology behavior, and coverage
- `references/quality-gates.md` — final source, story, Japanese, dialogue, AI-style, genre, and learning QA
