---
name: stealth-learning-short-fiction
description: Use this skill when the user wants a short, engaging Japanese story, light-novel-style reading passage, genre fiction, or narrative learning material that naturally embeds exact target English sentences and their Japanese translations for memorization or test preparation. Suitable for slice-of-life, romance, sports, horror, mystery, SF, fantasy, isekai, comedy, suspense, and other genres. The story must remain primarily Japanese and work as entertainment even if the English inserts are removed.
---

# Stealth Learning Short Fiction

## Purpose

Create short Japanese entertainment fiction in which the reader becomes familiar with exact target English sentences and grammar through memorable story scenes rather than overt instruction.

The primary product is a **good short story**. Learning is embedded underneath the story design.

This skill is not limited to fantasy or isekai. Genre should change with the user's request, the target sentences, and the emotional effect that best fits them.

## Core Principle

> Story first. Exact target sentences second. Explanation last.

A finished story must pass both tests:

1. **Story-First Test** — if every English target sentence and translation is removed, the remaining Japanese text is still an enjoyable, coherent short story.
2. **Memory-Anchor Test** — each target sentence is attached to a distinctive scene, emotion, action, revelation, joke, fear, victory, or relationship beat that can help the reader remember it later.

If either test fails, revise before delivery.

## Source Grounding

When the user supplies a textbook, test, example bank, worksheet, PDF, DOCX, image, or other source:

- Treat the supplied material as authoritative for the target sentences and test scope.
- Extract the target English exactly from the source.
- Do not silently modernize, simplify, paraphrase, correct, or replace a target sentence.
- If a source sentence appears erroneous or ambiguous, preserve it for exact-test practice but flag the concern separately instead of silently changing it.
- Use the source's Japanese translation when the user wants faithful reproduction; otherwise a natural Japanese translation may be used only when this does not alter the target meaning.
- Do not invent grammar rules or test coverage not supported by the supplied material.

Maintain an internal target-sentence ledger before drafting. See `references/target-sentence-embedding.md`.

## Default Reader Experience

Unless the user asks otherwise:

- The story is overwhelmingly Japanese.
- English appears only as short target-sentence inserts.
- Every target English sentence is immediately followed by its Japanese translation.
- Do not make Japanese characters suddenly speak English merely to insert a test sentence.
- Do not turn the story into a teacher-student grammar lecture.
- Do not append a grammar lesson, vocabulary list, comprehension quiz, or study notes unless the user requests them.
- Keep educational metadata, coverage logs, and QA notes out of the reader-facing story.

### Default Target Insert Format

Use a visually clean interruption at a meaningful moment:

**She might have sent the message to the wrong person.**  
彼女は間違った人にメッセージを送ってしまったかもしれない。

Then immediately return to the Japanese story.

The sentence may function as narration, a remembered line, a caption-like thought, a message, a report, a sign, an article line, an announcement, or another natural story object. It does **not** have to be spoken dialogue.

## Length Modes

Choose the shortest mode that can still produce a complete and satisfying story.

- **Micro:** about 400–700 Japanese characters; 1–2 target sentences; one scene, one turn.
- **Standard:** about 700–1,400 Japanese characters; 2–4 target sentences; default.
- **Extended:** about 1,400–2,200 Japanese characters; 3–5 target sentences; only when the story genuinely needs more room.

Do not pad a story to hit a word count. If too many target sentences are supplied, split them across multiple independent stories rather than stuffing them unnaturally into one story.

As a default, 2–4 exact target sentences per short story is preferred. Five is a soft maximum, not a goal.

## Workflow

### 1. Build the target-sentence ledger

Before inventing the plot, record for each target sentence:

- exact English
- exact or approved Japanese translation
- source location if known
- grammar/meaning focus supported by the source
- semantic situation expressed by the sentence
- whether exact wording is mandatory

Do not begin drafting until the exact strings are stable.

### 2. Choose the entertainment promise

Decide what makes this story worth reading **without considering the English yet**.

Specify internally:

- genre
- emotional promise: funny, tense, touching, romantic, eerie, cathartic, exciting, bittersweet, etc.
- protagonist's immediate want
- one obstacle or uncertainty
- one change, discovery, decision, reversal, or emotional payoff

If the premise is not interesting in one or two Japanese sentences, replace it.

### 3. Pick the smallest viable incident

Short fiction should usually cover one compact incident rather than a whole life arc.

Good scopes include:

- ten minutes after practice
- one train ride
- one late-night message
- one failed confession
- one forgotten umbrella
- one strange phone call
- one final pitch or serve
- one clubroom argument
- one hospital visit
- one abandoned classroom at night

Avoid unnecessary lore, backstory, side plots, large casts, or multiple twists.

### 4. Select a short-story shape

Use the compact five-beat model unless another structure clearly fits better:

1. **Hook** — create curiosity, tension, voice, surprise, or emotion in the opening 1–3 sentences.
2. **Situation** — establish the protagonist's immediate want or problem quickly.
3. **Pressure** — something complicates the situation, creates a misunderstanding, raises a small stake, or deepens emotion.
4. **Turn** — discovery, reversal, decision, realization, failure, success, scare, joke, or relationship shift.
5. **Aftertaste** — end with resonance appropriate to the genre: warmth, fear, laughter, ache, triumph, unease, or curiosity.

For slice-of-life, conflict can be small. For horror, the aftertaste may remain unresolved. For comedy, the final beat may be a punchline. For romance, it may be a small emotional shift rather than a confession.

See `references/short-story-craft.md` and `references/genre-presets.md`.

### 5. Assign each target sentence a story job

Never insert a target sentence merely because it must appear.

Give every target sentence at least one concrete function:

- reveals what is happening
- reveals what happened earlier
- changes how a character interprets events
- expresses a plan, prediction, obligation, possibility, regret, or memory
- becomes a clue
- raises or resolves a misunderstanding
- intensifies emotion
- marks a turning point
- anchors a repeated image or memory

If no natural job exists, move that sentence to another story.

### 6. Draft Japanese prose first

Draft the scene primarily in natural Japanese.

Use the existing Story Skills prose craft guidance, especially:

- `skills/chapter-writing/references/writing-guidelines.md`
- show rather than over-explain
- clear POV
- purposeful dialogue
- varied pacing
- sensory specificity
- a meaningful change by the end

When available, use the companion `better-writing` skill for prose quality and anti-generic checks.

### 7. Embed target sentences surgically

Insert the exact English only at the scene moment where it has the strongest semantic and emotional connection.

Immediately place the Japanese translation below it.

Do not:

- paraphrase an exact target
- split one target sentence into fragments unless the user explicitly asks
- force every sentence into spoken dialogue
- insert several target sentences back-to-back like a vocabulary list
- stop the story to explain the grammar
- surround the sentence with unnatural setup whose only purpose is to justify English

See `references/target-sentence-embedding.md`.

### 8. Perform entertainment revision

Revise the story once **ignoring the learning objective**.

Check:

- Would the first paragraph make a student continue reading?
- Is there a clear emotional or narrative question?
- Does something change?
- Are there unnecessary explanations?
- Is the dialogue alive rather than functional?
- Does the ending reward the setup?
- Is the tone faithful to the selected genre?

If not, improve the story before touching learning coverage.

### 9. Perform learning revision

Then verify:

- every required English sentence appears exactly
- every target has its Japanese translation immediately below it
- each target is attached to a memorable story beat
- no target's meaning is distorted by the surrounding Japanese
- grammar explanations have not invaded the story
- no unsupported rule has been added

### 10. Run the quality gates

Use `references/quality-gates.md` before delivery.

Do not deliver as final if the story feels like:

- a worksheet wearing a costume
- a grammar teacher disguised as a character
- a sequence of example sentences connected by filler
- an overcomplicated plot designed only to justify all targets

## Genre Selection

If the user specifies a genre, follow it.

If genre is unspecified, choose based on the target sentences and vary across outputs. Do not default to isekai, fantasy, romance, or any single genre.

Possible genres include:

- slice-of-life
- school comedy
- romance
- sports
- horror
- mystery
- suspense
- SF
- fantasy
- isekai
- family drama
- friendship
- workplace
- adventure
- bittersweet drama

Use `references/genre-presets.md` as a source of genre-specific craft, not as rigid templates.

## Output Rules

Reader-facing output should normally contain only:

1. title
2. story

Do not expose the target ledger, learning objectives, QA checklist, or grammar labels unless the user asks.

When generating several stories, make them meaningfully different in genre, premise, emotional rhythm, and ending shape. Do not simply reskin the same plot.

## Reference Files

- `references/short-story-craft.md` — compact storytelling techniques for hooks, turns, pacing, and endings
- `references/genre-presets.md` — genre-specific promises, plot pressures, and ending styles
- `references/target-sentence-embedding.md` — exact-sentence preservation and natural insertion strategy
- `references/japanese-prose-style.md` — natural Japanese narrative voice and anti-textbook rules
- `references/memory-design.md` — connect sentences to memorable scenes without overt teaching
- `references/quality-gates.md` — story-first, exactness, naturalness, and learning QA
