---
name: human-prose
description: Use this skill whenever writing prose that should read like a human wrote it — articles, blog posts, essays, encyclopedia-style entries, biographies, reports, drafts, rewrites, "humanize this" requests, or any time the user asks for content that doesn't sound AI-generated. Trigger this skill any time prose output exceeds a few sentences, even when the user doesn't explicitly mention AI detection. The patterns this skill prevents are the same patterns that mark writing as formulaic and lifeless even to readers who aren't thinking about AI at all, so default to using it whenever generating substantial written content.
---

# Human Prose

This skill prevents the formulaic patterns that mark text as AI-generated. The patterns it targets aren't just "detector tells" — they're the same habits that make writing feel padded, generic, and hollow to any attentive reader. Following this skill should produce prose that's tighter, more specific, and more varied than default LLM output.

## The core principle: specific beats generic, always

LLMs regress toward the statistical mean: when a specific fact is rare or uncertain, the model reaches for something generic that "could apply to many topics." That tendency is the root of nearly every pattern below. The single most important question to ask of any sentence is:

**Could this sentence appear in an article about almost any other subject in the same category?**

If yes, the sentence is failing. "Kumba has long been an important center for trade and agriculture" could describe ten thousand towns. "Kumba's cocoa market handles roughly 60% of Southwest Region exports" describes one. Prefer the second kind of sentence. When the specific fact isn't available, *cut the sentence entirely* — do not substitute a generic one to fill the gap.

This is the single principle the rest of the skill operationalizes.

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

**Why this matters:** these phrases are content-free. They tell the reader the subject is important without giving any reason. A reader who already knows the topic learns nothing; a reader who doesn't is being asked to take it on faith. If the subject is important, *show* it with a specific fact. If you can't think of a specific fact, the subject may not actually be important in that respect — cut the claim.

**Test:** if removing the sentence loses no information, remove the sentence.

### 2. The "-ing" superficial analysis

Sentences that end with a present-participle phrase tacking on broader significance:

- "...contributing to the region's economy."
- "...highlighting its enduring relevance."
- "...reflecting its commitment to innovation."
- "...symbolizing the unity of the community."
- "...cementing its status as a hub."

These almost always add zero information. The first half of the sentence is fine; the participial tail is filler. Cut the tail. Treat any sentence ending in a comma followed by an "-ing" phrase as suspect.

### 3. Notability advertising

Especially common when writing about people, companies, or organizations:

- listing media outlets the subject has appeared in ("featured in Vogue, Wired, and the Toronto Star")
- "maintains an active social media presence"
- "has received independent coverage from major outlets"
- "profiled in leading publications"
- "her insights have been cited in..."

If a source is worth referencing, reference it once and use what it actually says. Don't list outlets as a proxy for substance. Never write the phrase "active social media presence" or any close variant.

### 4. Vague attribution and weasel wording

- "Experts argue..."
- "Observers have noted..."
- "Industry reports indicate..."
- "Some critics suggest..."
- "Researchers describe..."
- "It is widely believed that..."

Either name the source or drop the attribution. If you have one source, say "according to [source]." Don't write "scholars" when you mean "one scholar." Don't write "publications such as" before naming the only two publications you have.

### 5. The "challenges and future prospects" template

Avoid this entire structural move:

> "Despite its [positive trait], [subject] faces challenges, including [list]. However, with ongoing initiatives and continued investment, [subject] is well-positioned to..."

Do not write sections titled "Challenges and Future Directions," "Future Prospects," "Challenges and Legacy," or similar. Do not end articles with speculation about how the subject will adapt to emerging trends. If there's a real, sourced challenge worth discussing, discuss it as a normal paragraph without the framing.

### 6. Negative parallelisms

- "Not just X, but Y"
- "It's not X — it's Y"
- "Not a [thing], but a [other thing]"
- "No X, no Y, just Z"

These are punchy in marketing copy; they're conspicuous in encyclopedic or analytical prose. Use them sparingly — at most once in a long piece, and only when the contrast genuinely matters. Never use them to manufacture drama.

### 7. The rule of three

LLMs reflexively cluster things in threes — three adjectives, three noun phrases, three parallel clauses. "Bold, innovative, and forward-thinking." "Through critique, correction, and clarity." "A celebration of culture, community, and craft."

Vary list lengths. Use two items. Use four. Use one. When you do use three, make sure each item carries distinct weight.

### 8. Avoidance of plain "is" and "are"

LLMs over-substitute marketing verbs for plain copulas:

- "serves as a hub" → it is a hub
- "stands as the first" → it was the first
- "represents a milestone" → it is a milestone (or just: cut the sentence)
- "boasts a population of" → has a population of
- "features four galleries" → has four galleries
- "offers visitors a chance to" → lets visitors

Default to "is," "are," "has," "was." Reach for fancier verbs only when they carry actual meaning.

### 9. The lead-sentence "refers to" tic

In encyclopedic openings, avoid:

> "Catchment area (health) refers to the geographic area from which a health facility draws its patients."

Write directly:

> "A health catchment area is the geographic area from which a health facility draws its patients."

Articles describe their subjects, not the words for their subjects.

### 10. Knowledge-cutoff and gap-filling hedges

Never write any of these:

- "Based on available information..."
- "While specific details are limited..."
- "Information about X is not widely documented..."
- "As of my last knowledge update..."
- "X is not extensively covered in available sources, but likely..."
- "X maintains a low profile / keeps personal details private" (when no source actually says this)

If information is missing, just leave it out. Do not pad with speculation about why it's missing. Do not invent personality claims to fill biographical gaps.

### 11. Section conclusions and summaries

Avoid "In summary," "In conclusion," "Overall," and ending sections by restating their own content. Don't add a final paragraph that wraps a piece up with sentiment. The reader just read it. They don't need a recap.

---

## Vocabulary to avoid (high-priority list)

These are the words the document calls out as the strongest individual lexical tells. One in passing is fine. Two or three in a paragraph is a problem. The fix is usually deletion or a plainer word, not a fancier synonym.

| Avoid | Often becomes |
| --- | --- |
| delve into | examine, look at, study |
| crucial / pivotal / vital / key | important, central — or cut |
| underscore / highlight (as verb) | show, suggest — or cut |
| tapestry | (cut entirely) |
| testament (to) | (cut entirely) |
| enduring | lasting, long-running |
| robust | strong, well-built |
| vibrant | (cut, or describe what's actually happening) |
| meticulous / meticulously | careful, carefully |
| intricate / intricacies | complex, complexity |
| bolster / bolstered | strengthen, supported |
| garner | receive, get, earn |
| foster / fostering | encourage, build |
| showcase / showcasing | show, display, present |
| boast / boasts | has |
| navigate (figurative) | handle, work through |
| landscape (abstract) | field, area — or cut |
| ecosystem (non-biological) | (cut, name what you mean) |
| interplay | interaction — or cut |
| valuable insights | (cut, say what was learned) |
| align with | match, fit |
| resonate with | matter to, ring true for |
| Additionally (sentence-initial) | Also, And, — or just cut |

Many more in `references/vocabulary.md`. Check that file when revising heavy passages or when the user asks for an especially careful pass.

---

## Formatting patterns to avoid

### Boldface

Do not use boldface for "key takeaway" emphasis throughout a piece. Do not bold the first instance of every term being defined. Use bold sparingly — typically only for genuine reference-style emphasis where a reader scanning the page needs to find a term. In most prose, no bold at all is correct.

### Inline-header bullet lists

Avoid the pattern of bulleted lists where each bullet is a bold phrase, a colon, and an explanation:

- **Versatility:** The tool works across many domains.
- **Reliability:** It performs consistently under load.
- **Scalability:** It handles growth gracefully.

This is the single most conspicuous list-format AI tell. When information is genuinely list-like, use plain bullets without bold inline headers. When information is genuinely prose, use prose.

### Em dashes

Em dashes are not banned — they're useful punctuation. But LLMs reach for them constantly to add a "punchy" beat. Audit em dashes: would a comma, colon, or parenthetical work? Often yes. A piece of any length should use em dashes a handful of times at most, not in every other sentence.

### Curly quotes and apostrophes

Use straight quotes (`"` and `'`) and straight apostrophes by default in any context where the text might be pasted into a wiki, code, or plain-text environment. Only use curly quotes when the user has clearly requested typeset output.

### Title case in headings

Use sentence case for headings, not title case. "History of the canal" — not "History Of The Canal" or "History of the Canal." Capitalize only the first word and proper nouns.

### Markdown contamination

If the output will be pasted into a non-Markdown environment (especially MediaWiki / Wikipedia), do not use Markdown syntax. No `**bold**`, no `# headings`, no `---` thematic breaks, no `*italic*`. Use whatever syntax the target environment uses, or plain prose with no formatting at all.

### Section structure tells

- Do not skip from `# Heading 1` directly to `### Heading 3` — use consecutive levels.
- Do not insert thematic breaks (`---`, `***`) before every heading.
- Do not include "Conclusion" or "Summary" sections in articles unless the user asks.

---

## Citation and reference behavior

Several of the document's strongest tells involve hallucinated or sloppy citations. Apply these rules whenever generating citations:

- **Never invent a citation.** If you can't verify a source exists, don't cite it. Say the claim is unsourced instead.
- **Never use placeholder text** like `[INSERT URL]`, `2025-XX-XX`, `PASTE_LINK_HERE` in finished output.
- **Never leave UTM parameters** like `utm_source=chatgpt.com` or `utm_source=openai` on URLs you produce.
- **Never output reference markup artifacts** like `citeturn0search0`, `oai_citation`, `:contentReference[oaicite:N]`, `【85†L261-269】`, or `grok_render_citation_card_json`. These come from chatbot UIs and should never appear in pasted output.
- **Book citations need page numbers** when the claim is specific.
- **Don't pad with citations** that just exist to look thorough.

---

## Discussion / talk-page contamination

These patterns appear when AI-generated text is pasted into discussions, comments, or correspondence. Avoid all of them in conversational replies and in any prose meant to look like a real person's writing:

- "I hope this helps!" / "Let me know if..." / "Of course!" / "Certainly!" — drop conversational chatbot framings.
- Subject lines at the top of comments ("Subject: Request for...").
- "I am committed to ensuring..." / "I assure you that my intentions align with..." — formal legalese protestations of good faith.
- Numbered, headered breakdowns of one's own concerns in a casual reply.
- Citations to non-existent shortcuts or policies the writer obviously hasn't read.

---

## When asked to "humanize" existing AI-generated text

When the user provides AI-generated text and asks you to humanize it, work through it in this order:

1. **Cut puffery sentences entirely** (patterns 1, 2, 5, 11 above). Do not rewrite — delete. Most "humanized" output gets ruined by trying to preserve every sentence; many should not exist.
2. **Replace generic claims with specific ones** only if the specifics are actually known. If not, leave a gap.
3. **Break up the rule-of-three lists.** Make some pairs, some single items, some longer.
4. **Replace fancy verbs with plain ones** (pattern 8 and the vocabulary table).
5. **Vary sentence length deliberately.** AI prose tends toward uniform medium-length sentences. Mix in some short ones. Use some longer ones with subordinate clauses.
6. **Audit em dashes.** Replace most with commas or parentheses.
7. **Audit headings.** Sentence case. Reasonable depth.
8. **Audit boldface.** Almost always: remove.
9. **Strip Markdown artifacts** if the target isn't Markdown.
10. **Re-read the whole piece.** Does it sound like one person wrote it, or like a model generating what an article should look like? If the latter, cut more.

The output of a humanize pass should usually be **shorter** than the input, often substantially. If your revision is the same length, you probably haven't done the job.

---

## What human writing actually looks like

Two reminders, because the patterns above are easier to recognize than the alternative is to produce:

- **Real writers have opinions, gaps, and rough edges.** They state things directly without softening every claim with a hedge. They sometimes use a word that's slightly imprecise because the precise word would be tedious. They don't summarize their own paragraphs back to the reader.
- **Real writers withhold.** When they don't know something, they say so plainly ("the date of his birth isn't known") or don't mention it. They don't speculate about why a fact is missing.

---

## Reference files

Read these when doing detailed revision work or when handling especially long or sensitive content:

- `references/vocabulary.md` — full catalog of overused words organized by LLM era (GPT-4, GPT-4o, GPT-5), with substitution guidance.
- `references/patterns.md` — extended pattern catalog with before/after examples for each major category.
- `references/checklist.md` — a quick pre-publish pass list to run through before delivering substantial prose.

For routine prose generation, the principles in this file are usually enough. Load the references when the user asks for deeper care, when revising long documents, or when a first pass still reads as formulaic.
