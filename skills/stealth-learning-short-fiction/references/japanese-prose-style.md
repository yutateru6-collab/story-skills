# Japanese Prose Style

The default output is a Japanese entertainment story, not a translated English exercise.

This file defines generation-time style constraints. Before delivery, always run the stricter revision pass in `natural-japanese-fiction-pass.md` and the dialogue rules in `character-voice-dialogue.md`.

## 1. Natural Japanese first

Write as contemporary Japanese fiction suitable for teenage readers unless the user specifies a different audience.

Prefer:

- natural sentence rhythm
- concrete verbs
- concise dialogue
- character-specific reactions
- ordinary Japanese used precisely
- sensory detail only where useful
- paragraphs that are easy to read on mobile

Avoid:

- textbook-like explanation
- unnatural literal translation prose
- overly formal narration unless genre requires it
- repetitive subject marking with 私は / 彼は / 彼女は
- excessive summary of emotion
- generic AI-like moralizing
- trying to sound "light-novel-like" through surface tricks alone

Naturalness outranks cleverness.

## 2. Keep the story overwhelmingly Japanese

English target blocks are accents, not the main narrative language.

Do not make the entire story bilingual line by line.

Do not insert English filler beyond the approved target sentences unless the user asks.

When no natural English-speaking context exists, the target may appear as a separated reader-facing learning block at the semantically matching point. Do not make Japanese characters suddenly speak or type English only to justify the target.

## 3. Light-novel readability without mannerisms

Use light-novel-like readability when appropriate:

- quick orientation
- clear voice
- readable paragraph breaks
- dialogue with subtext
- vivid but economical imagery
- hooks and turns

Do **not** treat these as mandatory mannerisms:

- chains of one-sentence fragments
- constant rhetorical questions in inner monologue
- a joke or metaphor at the end of every paragraph
- exaggerated self-commentary
- repeated `……` or `――`
- perfectly timed comeback dialogue in every exchange
- generic romantic shorthand such as repeated heart-pounding / face-heating narration

Do not imitate any living author or copyrighted franchise style. Build an original voice appropriate to the requested genre.

## 4. Dialogue is character-specific

Before writing dialogue, apply `character-voice-dialogue.md`.

Do not generate dialogue from a generic category such as "teenage boy," "girl," "best friend," or "anime character." Lock the actual character's age, personality, relationship distance, status, usual directness, teasing level, politeness, address terms, and emotional state.

The same character must change register depending on the listener.

A line that is natural Japanese can still be wrong for the character. Treat that as a failure.

Avoid characters saying things they both already know merely for reader exposition.

Use action beats when they reveal emotion or control pacing.

Realistic dialogue does not need a witty response every turn. Allow plain answers, silence, incomplete thoughts, missed timing, and physical reactions.

Avoid overusing:

- 「えっ？」
- 「なるほど」
- 「つまり」
- 「ということは」

especially when these lines only introduce explanations.

## 5. Japanese syntax over English syntax

Build sentences from the Japanese situation, not from an English-shaped logical template.

Avoid translationese such as:

- unnecessary explicit subjects
- heavy 無生物主語 + 他動詞 constructions
- nested relative-clause-like noun modification
- 「それは〜だ。なぜなら〜」 where ordinary Japanese would connect the reason directly
- 「〜することができる」 where a natural potential form works
- 「〜することによって」 where 「〜すると／〜して」 works
- abstract `have`-style phrases when more direct Japanese is available
- English-style double-dash insertions

If a sentence feels translated, reconstruct it from the situation instead of swapping synonyms.

## 6. Rhythm and sentence endings

Vary sentence length according to thought and action, not according to a style formula.

Short sentences are for genuine emphasis. Do not use fragment chains as the default rhythm.

Check repeated sentence endings, especially three or more nearby uses of:

- 〜だった。
- 〜した。
- 〜いる。
- 〜と思った。
- 〜気がした。

Sometimes the solution is to merge sentences, omit an obvious subject, or change the underlying construction—not merely replace the ending.

## 7. Do not explain grammar inside the fiction by default

Forbidden default patterns include:

- 「これは現在完了だ」
- 「この場合は過去進行形を使う」
- 「ポイントは〜」
- teacher character delivering a grammar lecture

The target sentence should gain meaning through the event itself.

Grammar explanation may be added separately only when the user asks.

## 8. Keep exposition proportional to length

For micro and standard stories, explain only what is necessary to understand:

- who matters
- what they want
- what is happening now
- what changed

Do not explain the full history of a club, family, fantasy kingdom, company, or relationship unless the payoff requires it.

Do not repeat information in narration after dialogue or action has already made it clear.

## 9. Emotional specificity without over-explaining

Replace vague declarations with observable behavior where possible.

Instead of:

> 彼はとても悲しかった。

consider a specific action, silence, object, or physical reaction appropriate to the character.

Do not ban direct emotion words entirely. Use them when they are the clearest choice.

Once the reader can infer the emotion, stop. Do not add a second paragraph explaining what that reaction means.

## 10. Endings

Do not close with a school-essay moral or an AI-style quotable summary.

Avoid:

- 「この経験から大切なことを学んだ。」
- 「英語は大切だと思った。」
- 「これからも頑張ろうと思った。」
- a generic line explaining the emotional theme after the real ending has already landed

Prefer an action, image, line of dialogue, decision, joke, chill, or echo that embodies the change.

## 11. Genre controls voice

- Comedy: quicker cuts, precise timing, less explanation after punchline
- Horror: restrained explanation, concrete sensory unease, controlled ambiguity
- Romance: subtext, small gestures, timing, vulnerability; do not narrate every romantic signal
- Rom-com: chemistry plus imperfect timing; do not substitute nonstop prepared banter for intimacy
- Sports: physical detail, pressure, measurable stakes, earned reaction
- Mystery: precise observation, fair clues, restrained withholding
- Fantasy/SF: one or two vivid speculative details instead of lore dumps
- Slice-of-life: small stakes with emotional precision

## 12. Anti-generic pass

Before delivery, look for and revise:

- stock motivational phrases
- interchangeable character voices
- excessive adjectives
- repeated sentence endings
- unnecessary rhetorical questions
- vague "something changed inside me" language
- convenient coincidences that solve the plot
- dialogue that exists only to carry information
- dialogue that would sound equally plausible if speaker names were swapped

The prose should feel like a story written for this specific incident and these specific people, not a generic template with target sentences inserted.
