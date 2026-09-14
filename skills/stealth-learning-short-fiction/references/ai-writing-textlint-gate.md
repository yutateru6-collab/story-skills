# AI-Writing Textlint Gate

Use this gate as a **detector**, not as an automatic rewriter.

The purpose is to surface wording and formatting patterns that may make Japanese prose feel AI-generated, then let the fiction-specific review decide whether each finding is actually a problem in context.

## External detectors

When Node/textlint is available, use these two MIT-licensed presets together:

- `p1ass/textlint-rule-preset-ai-words-ja`
  - detects Japanese words and phrases that became comparatively common in AI-era writing
  - uses morphological analysis, so inflected forms can also match
  - useful for lexical AI-isms
- `textlint-ja/textlint-rule-preset-ai-writing`
  - detects structural AI-writing patterns such as mechanical list formatting, hype expressions, emphasis patterns, and English-like colon continuation
  - useful for document-level/form-level AI-isms

Example installation:

```bash
npm install --save-dev textlint textlint-rule-preset-ai-words-ja @textlint-ja/textlint-rule-preset-ai-writing
```

Example configuration:

```json
{
  "rules": {
    "preset-ai-words-ja": {
      "no-ai-words": {
        "severity": "warning"
      }
    },
    "@textlint-ja/preset-ai-writing": true
  }
}
```

For fiction, keep `preset-ai-words-ja` findings at warning level. Do not turn them into automatic errors.

## Why warning-only is mandatory for fiction

The lexical preset was built from words reported as increasing in AI-era Japanese writing, with a reference study based on large-scale Qiita article counts. That is useful evidence for technical/nonfiction prose, but it is **not a fiction corpus**.

Its built-in dictionary includes words that can be perfectly natural in fiction, such as literal uses of:

- 走る
- 壊れる
- 焼く
- 穴
- 事故
- 疑う
- 踏み込む
- 静かに + certain verbs
- 〜した瞬間

Therefore:

> A textlint hit means “inspect this wording,” not “replace this word.”

Never perform blind synonym substitution. That often makes fiction less natural.

## Three-level interpretation

Classify every lexical finding into one of these buckets.

### A. Literal / scene-necessary — usually KEEP

Examples:

- a character literally runs: 「駅まで走った」
- an actual machine breaks: 「時計が壊れた」
- an actual accident: 「交通事故」
- a character genuinely suspects someone: 「兄を疑った」

If the word is the simplest, most natural Japanese for the concrete event, keep it.

### B. Genre-natural but possibly overused — COUNT / REVIEW

Examples:

- 「〜した瞬間」 in suspense/horror/action
- 「静かに消えた」 in horror
- 「黙って」 in romance/drama

One use can be fully natural. Repeated use can become conspicuously AI-like or mannered.

Rule of thumb:

- first occurrence: inspect only
- repeated within a short story: strong warning
- repeated across several stories in a set: rewrite at least some instances unless repetition is deliberate

### C. Abstract/meta AI-ish wording — usually REWRITE unless character/genre truly needs it

High-signal examples in explanatory narration include words such as:

- 土台
- 核心
- 構図
- 線引き
- 切り分ける
- 破綻
- 落とし穴
- 定石
- 入口 used metaphorically
- 照合 / 突き合わせる in casual narrative explanation

These are not forbidden Japanese. The warning is that AI often chooses them when a plainer scene-specific phrase would sound more human.

Ask:

> Would this POV character naturally think this word here?

If not, rewrite from the concrete situation rather than swapping in a thesaurus synonym.

## Protected target blocks

For stealth-learning fiction, the exact English target sentence and its required Japanese translation are protected source material.

Do not let textlint rewrite them.

When linting:

1. make a temporary lint copy of the story
2. replace protected target blocks with neutral placeholders, or disable textlint around those blocks
3. lint only the authored Japanese fiction prose
4. discard the temporary copy after review

Source fidelity outranks the AI-writing lint gate.

## Recommended pipeline

Run this only after the story already passes the basic story and character-voice draft stages.

1. Draft the Japanese story.
2. Run `Natural Japanese Fiction Pass`.
3. Run `Character Voice Dialogue` pass.
4. Protect exact target English + required translations.
5. Run `textlint-rule-preset-ai-words-ja`.
6. When available, also run `@textlint-ja/textlint-rule-preset-ai-writing`.
7. Classify every finding as KEEP / REVIEW / REWRITE.
8. Rewrite only findings that are genuinely artificial in context.
9. Rerun lint once.
10. Perform a final read-aloud pass.

Do not chase zero findings. A natural story can legitimately contain flagged words.

## Failure modes

Automatic FAIL if the revision process does any of the following:

- replaces every flagged word mechanically
- changes character dialogue only to satisfy a detector
- removes a precise concrete verb and replaces it with vague wording
- alters an exact test sentence or required Japanese translation
- forces the story to have zero warnings
- makes prose more formal, abstract, or literary merely to avoid a flagged word

The detector exists to reveal habits, not to dictate style.

## Manual fallback when textlint cannot run

If the runtime cannot install or execute textlint, manually scan for the same categories:

- repeated abstract explanatory nouns
- metaphorical technical verbs
- repeated `〜した瞬間`
- repeated `静かに + change/disappearance verb`
- AI-like hype or slogan lines
- mechanical bold/emoji/list formatting
- English-like colon continuation

Then apply the same KEEP / REVIEW / REWRITE judgment.

## Relationship to other gates

This gate supplements, but does not replace:

- `natural-japanese-fiction-pass.md`
- `character-voice-dialogue.md`
- `quality-gates.md`

A story can pass textlint and still sound artificial. Conversely, a good story can contain legitimate textlint warnings.
