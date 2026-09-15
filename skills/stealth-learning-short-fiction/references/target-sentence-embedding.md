# Target Sentence Embedding

This reference governs how exact English test sentences are inserted into Japanese entertainment fiction.

## 1. Exactness comes first

When a target sentence is marked exact or comes directly from a supplied test/example bank:

- preserve capitalization
- preserve auxiliaries
- preserve tense/aspect
- preserve articles
- preserve prepositions
- preserve word order
- preserve punctuation when practical
- preserve contractions if they are part of the source

Do not improve style, simplify, modernize, or replace vocabulary.

If the source itself appears inconsistent or wrong, do not silently repair it. Flag it outside the reader-facing story.

## 2. Build a sentence ledger

For every target, record internally:

```md
ID: T01
English: [exact sentence]
Japanese: [exact or approved translation]
Source: [test / lesson / line if known]
Meaning focus: [source-supported meaning]
Grammar focus: [source-supported point]
Semantic scene: [what kind of event naturally expresses this sentence]
Story job: [reveal / plan / clue / regret / action / etc.]
Exact: yes/no
Used: no
```

Mark `Used: yes` only after exact-string verification.

## 3. User-selected range defines the target set

Do not impose a fixed target count.

If the user selects 3 targets, use those 3.
If the user selects 8 targets, use those 8.
If the user selects 11 targets, use those 11.

Unless the user explicitly requests multiple stories, the selected set belongs to one story.

Never:

- split automatically at five targets
- repeat an earlier target merely to fill a quota
- invent a target to equalize story size
- omit an inconvenient target without telling the user

## 4. Reader-facing format

Default format:

**Exact English sentence.**  
自然な日本語訳。

Then return immediately to Japanese prose.

Do not label it `例文`, `文法ポイント`, `今回の表現`, or `暗記` unless the user explicitly asks for a study-facing format.

## 5. The surrounding story must make the sentence meaningful

A target insert should answer or intensify something the reader already cares about.

Strong placements:

- just after a character notices a crucial fact
- at the moment a plan is revealed
- during a memory that changes interpretation
- when a regret becomes clear
- when a rumor gains or loses credibility
- after a sports result changes the protagonist's decision
- when a frightening fact is confirmed
- when a relationship misunderstanding shifts

Weak placements:

- random paragraph break with no connection
- several unrelated target sentences in sequence
- a character reciting textbook sentences for no reason
- artificial exchange-student dialogue inserted only to justify English
- a brand-new mini-incident created only because another target remains

## 6. The English does not need to be spoken dialogue

Possible forms include:

- narrator-like emphasis
- subtitle/caption-like line
- internal remembered wording
- phone message
- email
- school notice
- stadium announcement
- article/report
- journal entry
- scoreboard commentary
- system notification
- letter
- poster/sign
- quoted statement

Choose the form that requires the least explanation.

## 7. Japanese remains the narrative language

The story should still read naturally if the target blocks are visually removed.

Do not build long English conversations unless the user asks for bilingual fiction.

Do not require readers to understand the English before the Japanese story can continue. The translation immediately below the target prevents comprehension friction.

## 8. Translation rules

By default, place one natural Japanese translation immediately below each English target.

If the user provided an official/example-bank translation and memorizing that translation matters, preserve it.

If no official translation exists:

- translate the meaning accurately
- keep Japanese natural
- avoid adding grammar explanation inside the translation
- avoid translating one sentence into several explanatory sentences

## 9. Story-job mapping

Useful mappings by meaning:

### Habit / general fact
Embed in routine, reputation, recurring practice, family habit, schedule, or stable world fact.

### Ongoing action
Embed in a live scene already in progress.

### Completed past
Embed in recollection, result report, alibi, diary entry, or completed event.

### Past-in-progress
Embed in interruption or simultaneous-event scenes.

### Present perfect / connection to now
Embed in continuing situation, accumulated experience, recent completion with current relevance, or state resulting from earlier action.

### Past perfect
Embed where one past event clearly precedes another past reference point.

### Future / plan / prediction
Embed in decisions, arrangements, schedules, forecasts, promises, threats, or evidence-based predictions as supported by the target.

### Modals
Embed in obligation, advice, possibility, certainty, prohibition, regret, or speculation according to the source meaning.

These mappings guide scene choice; they are not substitutes for the source's actual grammar notes.

## 10. Avoid fake naturalness

Do not create elaborate excuses for why a target appears in English.

Bad strategy:

- introduce a foreign exchange student solely to say one sentence
- make a teacher suddenly quiz the protagonist
- invent an English-learning contest to justify every line

Preferred strategy:

- accept the bilingual insert format as part of the reading design
- tie the meaning strongly to the scene
- keep the story itself natural

## 11. Density and spacing are variable

Target density depends on:

- how many targets the user selected
- how semantically compatible they are
- genre pacing
- how much emotional setup is required
- total story length

Do not use a fixed `maximum five targets` rule.

Instead:

- scale story length with target count
- space targets according to story beats
- combine semantically related targets inside the same incident when natural
- use internal scene breaks for larger target sets while preserving the same protagonist/problem
- if density feels too high, lengthen or redesign the story before splitting it

Multiple stories are a user-driven mode, not an automatic density fix.

## 12. Do not cluster targets mechanically

Useful functions include:

- establish situation
- deepen relationship
- complicate a plan
- reveal history
- create or confirm a clue
- intensify pressure
- trigger regret
- change a decision
- reinforce an outcome

Assign each target a function that belongs to the story already being told.

## 13. Exact-string QA

Before delivery:

1. compare every target against the authoritative source character by character
2. verify no word is missing or duplicated
3. verify tense and auxiliaries
4. verify translation is directly below the correct target
5. verify every target in the selected range is present unless the user requested a subset
6. verify surrounding Japanese does not imply a contradictory meaning
7. verify no source target was silently changed for naturalness
8. verify the story was not automatically split due to target count

If exactness cannot be verified, do not claim the story is final.
