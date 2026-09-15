# Quality Gates

A story is not finished merely because all target sentences are present.

Run all applicable gates before delivery.

## Gate A — Source Fidelity

Pass only if:

- every required target sentence in the user's selected range matches the authoritative source exactly when exactness is required
- every target has the correct Japanese translation directly below it
- no unsupported grammar rule or test-scope claim has been added
- any source ambiguity or likely error is flagged outside the story rather than silently changed
- no source target was omitted because it was inconvenient to fit

Fail if the story contains a `better` sentence that is not the actual test sentence.

## Gate B — Story-First Test

Temporarily remove all English target blocks and translations.

Ask:

- Does the Japanese story still make sense?
- Is there still a hook?
- Does the protagonist still want something?
- Does pressure accumulate?
- Does something change?
- Does the ending still land?

If removing the targets destroys the story, the story is too dependent on instructional scaffolding. Rewrite.

## Gate B2 — Selected-Range Unity

Unless the user explicitly requested multiple stories, pass only if the selected range functions as **one story**.

Fail when:

- the output silently becomes batches of five targets
- the protagonist/world resets after a fixed number of targets
- several unrelated mini-stories are joined under one title
- scene changes exist only to accommodate leftover target sentences
- characters disappear as soon as their target sentence has been used
- emotional investment repeatedly returns to zero

For a larger target set, prefer increased length and connected scene breaks before considering a split.

## Gate C — Natural Japanese / Native-Japanese Test

This gate is mandatory. Read and apply `natural-japanese-fiction-pass.md` before deciding PASS.

Pass only if:

- narration is not a literal-English translation style
- Japanese word order feels native rather than clause-by-clause translated
- obvious subjects and objects are omitted naturally where context allows
- sentence endings do not repeat mechanically
- paragraph rhythm is varied without relying on chains of one-line fragments
- punctuation is structural rather than decorative
- exposition is proportionate to length
- no teacher-like commentary leaks into ordinary narration
- no generic moral is attached to the ending
- no conspicuous `AI cleverness` is inserted only to sound witty, emotional, or light-novel-like
- inner monologue does not restate and then explain what the reader already understood
- the prose survives a mental read-aloud without awkward word order

Automatic warning patterns:

- repeated fragment chains such as noun / noun / reaction / punchline
- several paragraphs ending with quotable one-liners
- repeated rhetorical question -> self-answer inner monologue
- generic romance signals repeated in narration
- repeated dramatic markers: `……`, `――`, exclamation marks, one-sentence paragraphs
- cliché closing abstractions unless strongly earned by character voice

Fail if the Japanese is grammatically correct but still sounds noticeably generated, translated, mannered, or like a parody of light-novel prose.

When uncertain, prefer quieter, plainer Japanese that fits the character.

## Gate C2 — Character Voice & Dialogue

This gate is mandatory whenever the story contains dialogue. Read and apply `character-voice-dialogue.md` before deciding PASS.

Pass only if:

- every speaking character has an internal voice card
- age/life stage is reflected naturally without forced slang
- relationship to the listener affects wording and politeness
- address terms are consistent unless a deliberate change matters to the scene
- personality is visible through choices, omissions, timing, and directness—not catchphrase gimmicks
- emotion modifies the character's normal register plausibly
- dialogue sounds spoken rather than written
- shared-history exposition is not put into characters' mouths
- no character perfectly diagnoses another person's hidden feelings merely for reader convenience
- dialect is used only when grounded
- gender stereotypes are not being used as the voice generator

### Mandatory substitution test

Take several important lines and swap speaker labels.

If most lines still sound equally plausible coming from another character, FAIL and revise the voices.

### Mandatory listener test

Imagine the same character saying an important line to a different listener: best friend, crush, teacher, parent, senior, stranger.

If the wording would remain unchanged despite a major relationship difference, check for generic dialogue and revise when appropriate.

### Mandatory aloud test

Read the exchange mentally at conversational speed.

FAIL if:

- a high-school student sounds like an adult explanatory script
- a line is too polished for the emotional state
- every response is a perfectly timed comeback
- casual friends speak in uniformly neutral complete sentences without a character reason
- both characters have the same sentence rhythm
- a line feels natural on paper but unlikely to leave a person's mouth

## Gate C3 — AI-Writing Detector / textlint Review

Read and apply `ai-writing-textlint-gate.md` before deciding PASS.

When a Node/textlint runtime is available, use the external detectors described there:

- `p1ass/textlint-rule-preset-ai-words-ja` for lexical AI-like wording
- `textlint-ja/textlint-rule-preset-ai-writing` for structural AI-writing patterns

Important: for fiction, detector output is **warning evidence**, not an automatic rewrite command.

Before linting, protect exact target English sentences and required Japanese translations. Lint only the authored Japanese fiction.

Classify each finding as:

- **KEEP** — concrete/literal wording that is the natural expression for the scene
- **REVIEW** — genre-natural wording that may become mannered when repeated
- **REWRITE** — abstract/meta wording or templated phrasing that does not belong to the POV character or scene

Do not aim for zero warnings.

Automatic FAIL if the revision process:

- blindly replaces every flagged word
- changes a character's natural speech merely to satisfy textlint
- replaces a precise concrete verb with vague wording
- alters a protected test sentence or translation
- makes the prose more formal or abstract just to remove a warning

Pay special attention to frequency, not only presence.

If textlint cannot run in the current environment, perform the manual fallback in `ai-writing-textlint-gate.md`.

## Gate D — Target Naturalness

For each target sentence:

- Is the surrounding scene semantically compatible with the target?
- Does the target perform a story job?
- Is the English placement understandable without an artificial excuse?
- Does the Japanese translation fit the scene?
- Does the target connect to the same central incident, relationship, conflict, or emotional line as the rest of the selected range?

If no natural in-story English context exists, use a separated reader-facing target block at the matching moment. Do not invent an English chat, announcement, or conversation merely to justify the sentence.

If a target has no natural job, **redesign the plot or scene order first**. Do not automatically move it to another story.

## Gate E — Entertainment

Evaluate independently from educational coverage.

A strong story should have most of the following:

- opening curiosity within 1–3 sentences
- a concrete scene-level desire or concern
- pressure, uncertainty, or emotional friction
- a turn, discovery, decision, scare, joke, success, or failure
- a specific ending with emotional aftertaste
- at least one detail that belongs specifically to this story
- enough time with the protagonist/relationship/problem for the reader to care

Fail if the story is merely `correct` but dull.

## Gate F — Simplicity and Length Fit

Check for unnecessary complexity.

Warning signs:

- too many major characters for the story length
- several locations with little payoff
- multiple unrelated twists
- long worldbuilding explanation
- backstory longer than the live scene
- plot devices invented only to accommodate target sentences

Simplify before increasing complexity.

But do **not** remove required targets from the user's selected range merely to make the story shorter.

If the target set is dense:

1. remove redundant exposition and secondary complications
2. combine compatible targets into the same incident
3. increase story length within the variable-length guidance
4. use connected scene breaks
5. redesign the central premise if necessary

Automatic splitting is not a simplification strategy.

## Gate G — Genre Integrity

Pass only if the story delivers the genre's promise.

Examples:

- Horror must create unease or fear, not just contain a ghost.
- Sports must contain effort, pressure, competition, or physical stakes, not just mention a sport.
- Romance must contain vulnerability, anticipation, intimacy, or relational movement, not just a crush.
- Rom-com must contain relational movement and comic timing.
- Comedy must actually contain comic timing or payoff.
- Mystery must contain a fair question and meaningful clue/reveal.
- Slice-of-life must reward attention to small human detail.

Do not rely on costumes and scenery alone to signal genre.

## Gate H — Variation Across Multiple Stories

Use this gate only when the user actually requested multiple stories.

Compare them side by side.

Fail if several stories repeat:

- the same hook rhythm
- the same protagonist personality
- the same misunderstanding
- the same final twist
- the same message-app setup
- the same mentor lecture
- the same emotional arc
- the same sentence-fragment rhythm
- the same `clever` first-person voice
- the same friend/sidekick voice regardless of character

Do not invoke this gate as a reason to split one requested range into multiple stories.

## Gate I — Memory Anchor

For every target, write an internal one-line recall cue.

Example form:

`T03 -> empty gym / rival knew about morning practice`

Pass only if the cue is specific and clearly connected to the sentence's meaning.

If the cue is generic, strengthen the scene.

Distinct anchors do not require distinct mini-stories. Several targets may have different anchors inside the same central incident.

## Gate J — No Worksheet Costume

Automatic fail patterns:

- characters explicitly announce grammar labels without story reason
- a teacher walks in to explain the target
- targets are listed consecutively with filler between them
- each paragraph exists only to introduce another sentence
- each target gets its own unrelated mini-scene
- the final paragraph summarizes `what we learned`
- every target is spoken by a character despite unnatural context
- Japanese characters speak/type English solely because the author needs to place the target

Rewrite until the reader-facing artifact feels like fiction first.

## Gate K — Remove-the-Author Test

Ask whether the narrator is visibly trying too hard to entertain.

Temporarily mark every:

- witty metaphor
- self-deprecating joke
- dramatic fragment
- rhetorical question
- emotional explanation
- quotable final line

Then remove half of the marked items and reread.

If the story becomes more believable, keep the quieter version.

## Gate L — Length Scaling Check

Compare target count to story length.

Planning guide:

| Target sentences | Approximate Japanese story length |
|---:|---:|
| 1–2 | 800–1,400 characters |
| 3–4 | 1,400–2,200 characters |
| 5–6 | 2,200–3,200 characters |
| 7–9 | 3,200–4,500 characters |
| 10–12 | 4,500–6,000 characters |
| 13+ | scale upward as needed |

This is not a hard word-count gate.

FAIL when:

- the story is obviously padded to satisfy the table
- the story is so compressed that character investment cannot form
- targets arrive so frequently that the work reads like a worksheet
- the writer chose multiple stories merely because the target count exceeded five

## Final Delivery Check

Before calling the work final, verify:

- title is interesting without mentioning grammar unless requested
- requested genre is respected
- the user's selected source range is respected exactly
- target count is determined by the selected range, not by a fixed quota
- length is appropriate for target count and story needs without padding
- all exact targets are verified
- translations are directly below targets
- story remains primarily Japanese
- the selected range remains one story unless the user asked otherwise
- opening is strong
- ending is specific
- emotional investment accumulates instead of resetting
- mandatory Natural Japanese Fiction Pass was completed
- mandatory Character Voice & Dialogue pass was completed for all dialogue stories
- AI-writing detector/textlint review was completed when available, or manual fallback was used
- speaker substitution and aloud tests were applied to important dialogue
- English was not forced into implausible dialogue/chat
- no hidden QA notes appear in the reader-facing output
