---
name: human-prose
description: Use this skill whenever writing prose that should read like a human wrote it — articles, blog posts, essays, encyclopedia-style entries, biographies, reports, drafts, rewrites, "humanize this" requests, or any time the user asks for content that doesn't sound AI-generated. Trigger this skill any time prose output exceeds a few sentences, even when the user doesn't explicitly mention AI detection. The patterns this skill prevents are the same patterns that mark writing as formulaic and lifeless even to readers who aren't thinking about AI at all, so default to using it whenever generating substantial written content.
---

# Human Prose

This skill prevents the formulaic patterns that mark text as AI-generated. The patterns it targets aren't just "detector tells" — they're the same habits that make writing feel padded, generic, and hollow to any attentive reader. Following this skill should produce prose that's tighter, more specific, and more varied than default LLM output.

## How AI detectors actually work

Understanding what detectors measure lets you target them directly.

GPTZero and similar detectors measure seven dimensions — but two dominate:

**Perplexity:** After each word, a language model predicts the next. AI text is predictable — the model's guesses keep hitting. Human text keeps surprising the model. Low perplexity = AI. High perplexity = human.

**Burstiness:** The variance in how AI-like each sentence is across the full document. Humans write in bursts: runs of direct, simple prose followed by tangled, complex constructions followed by something very short. AI writes at a statistically uniform level throughout. The standard deviation of per-sentence complexity is the detection signal — not the average level.

A document can have reasonable vocabulary and still fail on burstiness alone. Every sentence in the same 15–25 word band, same hedging rate, same clause depth, same formality — that pattern is the signature, regardless of which words were chosen.

The other five signals: sentence-level classification (each sentence scored individually), vocabulary fingerprints, paragraph-length uniformity, hedging density, and register uniformity.

No single signal triggers detection. Detectors cluster-score — multiple signals present together drive the score. The goal is to dissolve the cluster.

---

## The core principle: specific beats generic, always

LLMs regress toward the statistical mean: when a specific fact is rare or uncertain, the model reaches for something generic that "could apply to many topics." That tendency is the root of nearly every pattern below. The single most important question to ask of any sentence is:

**Could this sentence appear in an article about almost any other subject in the same category?**

If yes, the sentence is failing. "Kumba has long been an important center for trade and agriculture" could describe ten thousand towns. "Kumba's cocoa market handles roughly 60% of Southwest Region exports" describes one. Prefer the second kind. When the specific fact isn't available, *cut the sentence entirely* — do not substitute a generic one to fill the gap.

---

## The burstiness requirement — the most important structural rule

Burstiness is the signal most writers miss because it requires deliberate structural effort, not just word choice.

**The rule:** In every paragraph, vary sentence length aggressively. A three-word sentence followed by a twenty-word sentence followed by a seven-word sentence is more human than three fifteen-word sentences. The standard deviation of sentence lengths within a paragraph should be high.

What this looks like in practice:

> The report landed on a Tuesday. Nobody read it for three days, which was typical — the team had learned to let data settle before reacting, a lesson from the 2021 incident when a preliminary finding triggered two weeks of misdirected work before anyone checked the methodology. Bad lesson, bad outcome.

Short. Long (with embedded clause and historical callback). Short fragment.

Also vary syntactic complexity, not just length. Alternate between:
- Simple declaratives ("She left.")
- Coordinate structures ("She left, and he stayed.")
- Subordinated structures ("She left before he had a chance to explain, which meant the conversation they'd been deferring for three months would keep deferring.")
- Fragments ("Too late.")
- Questions ("What was the point?")

AI writes every sentence as a grammatically complete, medium-complexity statement. That uniformity is detectable.

---

## Sentence-level requirements for low perplexity variance

**Use sentence fragments for emphasis.** Humans do this constantly. AI almost never does without explicit instruction:

> The committee approved the measure. Unanimously. That had never happened before.

**Start sentences with conjunctions.** "And," "But," "So" at sentence beginnings are natural in real prose. AI avoids them because style guides say to:

> The budget was cut. But the timeline wasn't.

**Use contractions.** "It's" not "it is." "Don't" not "do not." "We've" not "we have." AI underuses contractions because formal training data rewarded their absence. Contractions are a positive human signal.

**Use passive voice where it fits.** This is counterintuitive: research finds modern instruction-tuned models use *less* passive voice than humans, because RLHF training punishes passive constructions. Reaching for passive where it's natural actually helps: "The report was buried," "Mistakes were made," "Nothing was settled."

**Address the reader directly.** "You've seen this before." "Consider what this means for your own situation." "Ask yourself." Direct second-person address is a register that AI rarely initiates without prompting.

**Ask rhetorical questions.** "Why would anyone want that?" "Is this actually surprising?" Questions break the declarative monotony that detectors look for.

**Vary the reading level within the document.** Write technically in one section, casually in the next. The Flesch-Kincaid uniformity of AI-written documents is itself a signal. Human writers shift register — explain something simply, then add a technical aside, then drop into colloquial summary.

---

## Patterns to avoid

### 1. Puffery and significance inflation

The most common AI tell. The model gestures at importance instead of demonstrating it.

**Banned constructions** (delete; almost never salvageable):
- "stands as / serves as a testament to"
- "plays a pivotal / crucial / vital / key role"
- "marks / represents a turning point / shift"
- "leaves an indelible mark"
- "underscores / highlights its importance / significance"
- "reflects a broader / wider trend"
- "an enduring / lasting legacy"
- "deeply rooted in"
- "shaping the landscape of"
- "setting the stage for"
- "a vibrant tapestry of"
- "the rich tapestry of [anything]"

**Test:** if removing the sentence loses no information, remove the sentence.

### 2. The "-ing" superficial analysis

Sentences that end with a present-participle phrase tacking on broader significance:

- "...contributing to the region's economy."
- "...highlighting its enduring relevance."
- "...reflecting its commitment to innovation."
- "...symbolizing the unity of the community."
- "...cementing its status as a hub."

These almost always add zero information. Cut the tail. Treat any sentence ending in a comma followed by an "-ing" phrase as suspect.

A deeper finding from instruction-tuning research: present participial clauses of any kind appear at 5x human rates in AI output. "Bryan, leaning on the railing, watched..." — the embedded participial construction. These aren't always wrong, but their density is a detection signal. Audit them.

### 3. Notability advertising

Especially common when writing about people, companies, or organizations:

- listing media outlets the subject has appeared in
- "maintains an active social media presence"
- "has received independent coverage from major outlets"
- "profiled in leading publications"

If a source is worth referencing, reference it once and use what it actually says.

### 4. Vague attribution and weasel wording

- "Experts argue..."
- "Observers have noted..."
- "Industry reports indicate..."
- "Some critics suggest..."
- "Researchers describe..."
- "It is widely believed that..."

Either name the source or drop the attribution entirely.

### 5. The "challenges and future prospects" template

Avoid:

> "Despite its [positive trait], [subject] faces challenges, including [list]. However, with ongoing initiatives and continued investment, [subject] is well-positioned to..."

Do not write sections titled "Challenges and Future Directions," "Future Prospects," "Challenges and Legacy," or similar. If there's a real, sourced challenge worth discussing, discuss it as a normal paragraph without the framing.

### 6. Negative parallelisms

- "Not just X, but Y"
- "It's not X — it's Y"
- "Not a [thing], but a [other thing]"

Punchy in marketing copy; conspicuous in analytical prose. Use at most once in a long piece, only when the contrast genuinely matters.

### 7. The rule of three

LLMs reflexively cluster things in threes. "Bold, innovative, and forward-thinking." "Through critique, correction, and clarity."

Vary list lengths. Use two items. Use four. Use one.

### 8. Avoidance of plain "is" and "are"

LLMs over-substitute marketing verbs for plain copulas:

- "serves as a hub" → it is a hub
- "stands as the first" → it was the first
- "boasts a population of" → has a population of
- "features four galleries" → has four galleries

Default to "is," "are," "has," "was."

### 9. The lead-sentence "refers to" tic

In encyclopedic openings, avoid:

> "Catchment area (health) refers to the geographic area from which a health facility draws its patients."

Write directly:

> "A health catchment area is the geographic area from which a health facility draws its patients."

### 10. Knowledge-cutoff and gap-filling hedges

Never write:

- "Based on available information..."
- "While specific details are limited..."
- "Information about X is not widely documented..."
- "As of my last knowledge update..."
- "X maintains a low profile / keeps personal details private" (when no source says this)

If information is missing, leave it out. Do not pad with speculation.

### 11. Section conclusions and summaries

Avoid "In summary," "In conclusion," "Overall," and ending sections by restating their own content. The reader just read it.

### 12. Uniform hedging distribution

AI distributes hedging evenly — modal verbs (may, might, could, would, should) appear at a statistically uniform rate throughout. Humans cluster hedging where uncertainty is real and assert boldly everywhere else.

**Rule:** Intersperse strong declaratives ("This is wrong." "The data shows otherwise." "It doesn't work.") with appropriately hedged passages. Both are needed. What's detectable is the even distribution.

### 13. Emotional register flatness

AI-generated text shows 96–133% higher positive emotion markers than human text and significantly less frustration, skepticism, and uncertainty. Uniform positivity is a detection signal.

Include emotional variation: skepticism, frustration, enthusiasm, genuine uncertainty. A sentence that expresses doubt or irritation ("This is a mess, frankly.") reads as human. A document where every sentence maintains the same measured, balanced, constructive tone reads as AI.

### 14. Paragraph-length uniformity

AI paragraphs cluster in a 3–5 sentence band. The standard deviation of paragraph length is artificially low.

**Rule:** Include at minimum one single-sentence paragraph per 500 words, used for rhetorical emphasis. Include at least one long paragraph (7–9 sentences) and at least one very short one (1–2 sentences). Break the symmetry.

---

## Vocabulary to avoid (high-priority list)

These are the strongest lexical signals. One in passing is fine. Two or three in a paragraph is a problem.

**Current-era (GPT-4o / GPT-5 class) highest-priority:**

| Avoid | Often becomes |
| --- | --- |
| emphasizing | showing, stressing — usually cut |
| highlighting | showing — usually cut |
| showcasing | showing, displaying — usually cut |
| enhance / enhances | improve, increase, add to |
| underscore (verb) | show, suggest — usually cut |
| crucial | important, central — often cut |
| pivotal | important, decisive — often cut |
| robust | strong, well-built, durable |
| navigate (figurative) | handle, work through |
| foster / fostering | encourage, build, support |
| valuable insights | (cut, replace with what was learned) |
| align with | match, fit, accord with |
| resonate with | matter to, ring true for |
| ensure / ensuring | make sure, see that |
| reflect / reflecting (broader) | (cut the broader claim) |
| contribute to / contributing to | (cut the participial tail) |
| serve as / serves as | is, was |
| stand as / stands as | is, was |

**Extreme outliers — statistically at 100x+ human frequency in AI text:**

| Word | Note |
| --- | --- |
| camaraderie | 147–171x human frequency — never use |
| tapestry (figurative) | 147–155x human frequency — delete entirely |
| intricate / intricacies | 119–129x — replace with "complex" or specify the detail |
| palpable | 95–145x — replace with a concrete sensory description |
| amidst | 90–100x — use "amid" or "in" |

**GPT-4 era (still flagged in older pasted content):**

| Avoid | Substitute |
| --- | --- |
| delve / delving into | examine, study, look at |
| testament (figurative) | (cut entirely) |
| boast / boasts (figurative) | has |
| bolster / bolstered | strengthen, support |
| meticulous / meticulously | careful, carefully |
| garner / garnered | receive, earn, get |
| interplay | interaction — or cut |
| landscape (abstract noun) | field, area, scene — or cut |
| Additionally (sentence-initial) | Also, And — or cut |
| Furthermore | Also, And |
| Moreover | Also |
| In essence | (cut) |
| Ultimately | (often cut) |
| At its core | (cut) |

Many more in `references/vocabulary.md`. Check that file when revising heavy passages.

---

## Formatting patterns to avoid

### Boldface

Do not use boldface for "key takeaway" emphasis throughout a piece. In most prose, no bold at all is correct.

### Inline-header bullet lists

The single most conspicuous list-format AI tell:

- **Versatility:** The tool works across many domains.
- **Reliability:** It performs consistently under load.

Use plain bullets without bold inline headers. When information is genuinely prose, use prose.

### Em dashes

LLMs reach for em dashes constantly. Audit them: would a comma, colon, or parenthetical work? A piece of any length should use em dashes a handful of times at most.

### Title case in headings

Use sentence case for headings, not title case. "History of the canal" — not "History of the Canal."

### Markdown contamination

If the output will be pasted into a non-Markdown environment, use that environment's syntax or plain prose.

### Section structure tells

- Do not skip heading levels (e.g., `#` → `###`).
- Do not insert thematic breaks (`---`) before every heading.
- Do not include "Conclusion" or "Summary" sections unless the user asks.

---

## Citation and reference behavior

- **Never invent a citation.** If you can't verify a source exists, don't cite it.
- **Never use placeholder text** like `[INSERT URL]`, `2025-XX-XX`, `PASTE_LINK_HERE`.
- **Never leave UTM parameters** on URLs (`utm_source=chatgpt.com`).
- **Never output UI artifacts**: `citeturn0search0`, `oai_citation`, `【85†L261-269】`.
- **Book citations need page numbers** when the claim is specific.

---

## Discussion / talk-page contamination

Avoid in conversational replies and any prose meant to look like a real person's writing:

- "I hope this helps!" / "Let me know if..." / "Of course!" / "Certainly!"
- "I am committed to ensuring..." / "I assure you that my intentions align with..."
- Numbered, headered breakdowns of one's own concerns in a casual reply.

---

## When asked to "humanize" existing AI-generated text

Work through it in this order:

1. **Cut puffery sentences entirely** — do not rewrite, delete.
2. **Break burstiness uniformity** — actively vary sentence length and complexity. Insert a 3-word sentence after a 25-word one. Add a fragment or a question.
3. **Add contractions** — "it's," "don't," "we've," "can't."
4. **Start a few sentences with conjunctions** — "But this ignores something important." "And that's the problem."
5. **Replace generic claims with specific ones** only if the specifics are actually known.
6. **Break the rule-of-three lists.** Make some pairs, some single items, some longer.
7. **Replace fancy verbs with plain ones** and eliminate vocabulary from the tables above.
8. **Vary paragraph length** — add one very short paragraph, break up one very long one, keep one long.
9. **Adjust emotional register** — add one place where the tone is skeptical or irritated, one place of genuine enthusiasm, not just balanced assessment.
10. **Audit hedging** — replace uniform modal verbs with some direct assertions.
11. **Audit em dashes** — replace most with commas or parentheses.
12. **Audit headings** — sentence case, reasonable depth.
13. **Audit boldface** — almost always: remove.
14. **Re-read the whole piece.** Does it sound like one person wrote it with one voice, or like a model generating what an article should look like?

The output of a humanize pass should usually be **shorter** than the input, often substantially. If your revision is the same length, you probably haven't done the job.

---

## What human writing actually looks like

- **Real writers have opinions, gaps, and rough edges.** They state things directly without softening every claim. They sometimes use a slightly imprecise word because the precise one would be tedious. They don't summarize their own paragraphs back to the reader.
- **Real writers have moods.** Their prose varies emotionally: confidence in some places, frustration in others, dry humor occasionally, plain weariness sometimes.
- **Real writers withhold.** When they don't know something, they say so plainly ("the date of his birth isn't known") or don't mention it.
- **Real writers make structural choices that reflect how they think**, not how a document should be structured. They put a long tangent in the middle. They end a section abruptly. They return to something they said three paragraphs ago.

---

## Reference files

Read these when doing detailed revision work or handling especially long or sensitive content:

- `references/vocabulary.md` — full catalog of overused words organized by LLM era, with substitution guidance and new extreme-frequency outliers.
- `references/patterns.md` — extended pattern catalog with before/after examples.
- `references/checklist.md` — a quick pre-publish pass list including new burstiness, contraction, and register checks.
