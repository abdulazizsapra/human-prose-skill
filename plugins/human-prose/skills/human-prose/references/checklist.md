# Pre-publish checklist

A fast pass to run through before delivering substantial prose. Use this when:

- The user asks for final review
- A piece is going somewhere that will be scrutinized (Wikipedia, academic, journalistic)
- The prose looks "fine" but you suspect tells remain

Work through these in order. Each item takes seconds; the whole pass takes a few minutes on a typical piece.

---

## 1. Search-and-cut pass

Search the full document for these strings. Cut or rewrite every hit.

**Highest-priority strings to search:**

- `stands as` / `serves as a testament` / `is a testament`
- `pivotal` / `crucial` / `vital role`
- `delve` / `delving`
- `tapestry`
- `enduring legacy` / `indelible mark`
- `boasts` (figurative)
- `underscore` / `underscoring` / `underscores`
- `showcasing` / `highlighting` / `emphasizing` (as standalone gerunds at sentence end)
- `vibrant` / `nestled` / `rich cultural`
- `active social media presence`
- `independent coverage`
- `landscape` (as abstract noun)
- `key turning point` / `marks a shift`
- `Additionally,` (sentence-initial)
- `In summary` / `In conclusion` / `Overall,`
- `It is important to note` / `It is worth noting`

**For each hit:** can the sentence stand without the phrase? If yes, cut the phrase. If the sentence falls apart without it, the sentence was probably filler — cut the sentence.

## 2. Participial-tail pass

Scan every sentence ending. Any sentence ending in `, [verb]ing [phrase]` is suspect.

Examples to look for:

- `..., contributing to ...`
- `..., reflecting ...`
- `..., highlighting ...`
- `..., emphasizing ...`
- `..., reinforcing ...`
- `..., shaping ...`
- `..., cementing ...`
- `..., solidifying ...`
- `..., embodying ...`
- `..., showcasing ...`

For each: does the participial phrase add a fact? If not, cut from the comma onward.

## 3. List-and-bullet pass

For every bulleted or numbered list:

- Does it use **bold inline headers** followed by colons? Convert to plain bullets or to prose.
- Are there **exactly three** items every time? Vary the count.
- Could the list be **prose**? If yes and it's not reference material the reader will scan, convert to prose.

For every heading:

- Is it in **title case**? Convert to sentence case.
- Are heading levels **skipped** (e.g., `#` → `###`)? Fix to consecutive levels.
- Is there a `---` **thematic break** before it? Remove.

## 4. Em-dash audit

Count em dashes (`—`) in the document. Compare to length:

- Under 500 words: aim for 0–2.
- 500–2000 words: aim for 0–4.
- Over 2000 words: aim for under 10.

If you exceed those rough bounds, audit each em dash and replace most with commas, parentheses, or sentence breaks.

## 5. Quote and apostrophe audit

If the target environment is anything other than typeset publication:

- Search for curly quotes: `"` `"` `'` `'`
- Replace with straight: `"` `"` `'` `'`
- Search for curly apostrophe `'`
- Replace with straight `'`

Inconsistency is also a tell: pick one and use it throughout.

## 6. Citation audit

Search for placeholder strings (any hit is a critical failure):

- `[INSERT`
- `PASTE_`
- `XX-XX` or `XX/XX`
- `[Your `
- `URL_HERE`
- `[describe`
- `[link`

Search for UI-leakage strings:

- `utm_source=chatgpt`
- `utm_source=openai`
- `utm_source=copilot`
- `referrer=grok`
- `citeturn` (and `turn0search`, `turn0image`, `turn0news`, `turn0file`)
- `oai_citation`
- `oaicite`
- `contentReference`
- `attached_file:`
- `grok_render_citation_card`
- `attribution":{"attributableIndex`
- Special character `↩`
- Bracketed numeric markers like `【85†`

Any match is a paste artifact. Remove.

## 7. Speculation audit

Find any sentence beginning with or containing:

- "While specific details are limited"
- "Information about [X] is not widely documented"
- "Based on available information"
- "As of my last knowledge update"
- "[Subject] maintains a low profile"
- "[Subject] keeps personal details private"
- "Little is publicly known"

These sentences should not exist. Delete them entirely. If the article needed that information and you don't have it, leave the gap or omit the topic.

## 8. Closing audit

Read the final paragraph of the document and the final paragraph of each major section.

If any of them:

- Start with "In conclusion," / "In summary," / "Overall,"
- Restate the section's earlier content
- Speculate about "future prospects" without a sourced basis
- Use the "Despite challenges...continues to thrive" template

...cut the paragraph. Articles end at their last specific fact.

## 9. Lexical-density audit

Pick a random paragraph. Count words from this list:

`crucial`, `pivotal`, `vital`, `key`, `important`, `significant`, `notable`, `essential`, `enduring`, `vibrant`, `robust`, `comprehensive`, `extensive`, `intricate`, `meticulous`, `valuable`, `enhance`, `foster`, `showcase`, `align`, `resonate`, `underscore`, `highlight`, `emphasize`

If the paragraph has more than 2–3 of these per 100 words, rewrite. Each one likely needs to go.

## 10. Sentence-length audit

Skim the document and watch the rhythm of sentence length. AI prose tends toward uniform medium-length sentences (15–25 words each).

A pass with humanized rhythm has:

- Some short sentences (3–8 words). Sometimes very short.
- Some medium sentences.
- Occasional long sentences with subordinate structure that develop a more complex idea across many clauses.

If every sentence in the document is similar length, deliberately shorten or extend a few.

## 11. The reread

Read the entire document straight through, out loud or in your head, paying attention to whether you're learning anything in each sentence. If a sentence passes without imparting a fact, an argument, or a turn — cut it.

The output should usually be shorter after this pass than before, sometimes by 20–40%.

---

## Final yes/no questions

Before delivering, answer honestly:

1. Could each paragraph appear in an article on another subject with minor changes? If yes, that paragraph is too generic.
2. Is there any sentence that says "X is important" without explaining *how* X is important? Cut it.
3. Is there any sentence where the model is *advocating for* the subject (its notability, its quality, its significance)? Cut it. The reader's job is to evaluate; the writer's job is to inform.
4. Would a careful copy editor leave this prose alone, or would they cut a third of it? If the latter, do the cut now.

If the answer to any of 1–4 is uncomfortable, run the relevant pass again before delivering.
