# Pre-publish checklist

A fast pass to run through before delivering substantial prose. Use this when:

- The user asks for final review
- A piece is going somewhere that will be scrutinized (publication, academic, journalistic)
- The prose looks "fine" but you suspect tells remain
- The user has tested with GPTZero or a similar detector and gotten a high AI score

Work through these in order. Each item takes seconds; the whole pass takes a few minutes on a typical piece.

---

## 0. Burstiness check (run this first)

This is the primary detection signal and the one most writers miss.

Read through the document and count sentence words in each paragraph. If every sentence is between 12 and 25 words, you have a burstiness problem regardless of vocabulary.

**Fix:** In each paragraph, deliberately introduce:
- At least one sentence under 8 words (ideally 3–5)
- At least one sentence over 30 words with a subordinate clause
- Optionally: one fragment

**Check paragraph lengths too.** If every paragraph is 3–5 sentences, that uniformity is a detection signal. Aim for at least one paragraph of 1–2 sentences and one of 7–9 sentences in a 500+ word piece.

---

## 1. Search-and-cut pass

Search the full document for these strings. Cut or rewrite every hit.

**Tier-0 extreme outliers (delete on sight):**

- `camaraderie` (147–171× human frequency)
- `tapestry` (147–155× human frequency)
- `intricate` / `intricacies` (119–129× human frequency)
- `palpable` (95–145× human frequency)
- `amidst` (90–100× human frequency)

**Highest-priority strings to search:**

- `stands as` / `serves as a testament` / `is a testament`
- `pivotal` / `crucial` / `vital role`
- `delve` / `delving`
- `enduring legacy` / `indelible mark`
- `boasts` (figurative)
- `underscore` / `underscoring` / `underscores`
- `showcasing` / `highlighting` / `emphasizing` (as standalone gerunds at sentence end)
- `vibrant` / `nestled` / `rich cultural`
- `active social media presence`
- `landscape` (as abstract noun)
- `key turning point` / `marks a shift`
- `Additionally,` (sentence-initial)
- `Furthermore,` / `Moreover,`
- `In summary` / `In conclusion` / `Overall,`
- `It is important to note` / `It is worth noting`
- `seamlessly` / `transformative` / `multifaceted` / `nuanced` / `groundbreaking`
- `camaraderie` / `palpable` / `amidst`

**For each hit:** can the sentence stand without the phrase? If yes, cut the phrase. If the sentence falls apart without it, the sentence was probably filler — cut the sentence.

---

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

Also audit **mid-sentence participial constructions**: "Bryan, leaning on his experience, argued..." — these appear at 5× human rates in AI text. Not all are wrong, but review each one.

---

## 3. Contraction and informality pass

AI underuses contractions and informal constructions. Check whether the register warrants them; if so, add them.

**Contractions to consider adding:**
- "it is" → "it's" (in informal/moderate contexts)
- "do not" → "don't"
- "we have" → "we've"
- "cannot" → "can't"
- "they are" → "they're"
- "will not" → "won't"

**Informal sentence structures:**
- Does the piece start any sentence with "But," "And," "So," or "Yet"? If not and the context allows it, add one.
- Is there at least one fragment sentence used for emphasis? ("Too late." "Not quite." "Wrong.")
- Is there at least one direct-address sentence toward the reader? ("You've probably seen this." "Ask yourself.")
- Is there at least one rhetorical question?

These aren't required for all prose types — an academic paper warrants no contractions. But for blog posts, essays, articles, or any conversational content, their complete absence is a detection signal.

---

## 4. Hedging uniformity pass

Count the modal verbs in the document: may, might, could, would, should, perhaps, possibly, likely, probably.

**Problem pattern:** these appear at a statistically uniform rate throughout — every few sentences, one appears.

**Human pattern:** clusters near genuinely uncertain claims, absent near confident ones.

**Fix:** Find 2–3 places where the text hedges when it could assert. Replace "This may suggest that X" with "This suggests X" or "This shows X." Find one place to add a strong, direct, possibly provocative declarative sentence that makes no qualifications.

---

## 5. Emotional register pass

Read through and note the emotional tone of each paragraph. If the entire piece is:
- Measured
- Balanced
- Constructive
- Positive

...that uniformity is a detection signal. Real writing has emotional variation.

**Add at least one of:**
- A moment of skepticism or doubt ("This doesn't hold up.")
- A moment of frustration or criticism ("The argument is circular, and this seems to have escaped notice.")
- A moment of genuine enthusiasm, not just measured assessment
- A moment of admitted uncertainty

---

## 6. List-and-bullet pass

For every bulleted or numbered list:

- Does it use **bold inline headers** followed by colons? Convert to plain bullets or to prose.
- Are there **exactly three** items every time? Vary the count.
- Could the list be **prose**? If yes and it's not reference material the reader will scan, convert.

For every heading:

- Is it in **title case**? Convert to sentence case.
- Are heading levels **skipped** (e.g., `#` → `###`)? Fix to consecutive levels.
- Is there a `---` **thematic break** before it? Remove.

---

## 7. Em-dash audit

Count em dashes (`—`) in the document. Compare to length:

- Under 500 words: aim for 0–2.
- 500–2000 words: aim for 0–4.
- Over 2000 words: aim for under 10.

If you exceed those rough bounds, audit each em dash and replace most with commas, parentheses, or sentence breaks.

---

## 8. Passive voice check

Counterintuitively, AI uses *less* passive voice than humans. Modern instruction-tuned models were trained to prefer active voice, and detectors have measured this gap.

Scan for opportunities to use passive voice where it fits naturally:
- "The budget was cut." (not "They cut the budget.")
- "Mistakes were made." (not "The team made mistakes.")
- "Nothing was settled." (not "They settled nothing.")

Use passive where the agent is unknown, unimportant, or where the construction reads more naturally. Don't force it — but don't avoid it either.

---

## 9. Reading-level variation pass

AI maintains a statistically uniform Flesch-Kincaid reading level throughout a document. Humans shift register.

Read through and identify whether the document has sections that are notably more technical and sections that are notably more casual or direct. If the entire piece reads at the same complexity level, vary it:

- Add one section or paragraph that explains something in simpler, more direct terms than surrounding content.
- Add one technical or more demanding passage.
- Consider one colloquial aside in an otherwise formal document.

---

## 10. Quote and apostrophe audit

- Search for curly quotes: `"` `"` `'` `'`
- Replace with straight: `"` `"`  `'` `'`
- Search for curly apostrophe `'`
- Replace with straight `'`

---

## 11. Citation audit

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
- Special character `↩`
- Bracketed numeric markers like `【85†`

---

## 12. Speculation audit

Find any sentence beginning with or containing:

- "While specific details are limited"
- "Information about [X] is not widely documented"
- "Based on available information"
- "As of my last knowledge update"
- "[Subject] maintains a low profile"
- "[Subject] keeps personal details private"
- "Little is publicly known"

Delete entirely. Don't rewrite. If the article needs the information and you don't have it, leave the gap.

---

## 13. Closing audit

Read the final paragraph of the document and the final paragraph of each major section.

If any of them:

- Start with "In conclusion," / "In summary," / "Overall,"
- Restate the section's earlier content
- Speculate about "future prospects" without a sourced basis
- Use the "Despite challenges...continues to thrive" template

...cut the paragraph. Articles end at their last specific fact.

---

## 14. Lexical-density audit

Pick a random paragraph. Count words from this list:

`crucial`, `pivotal`, `vital`, `key`, `important`, `significant`, `notable`, `essential`, `enduring`, `vibrant`, `robust`, `comprehensive`, `extensive`, `intricate`, `meticulous`, `valuable`, `enhance`, `foster`, `showcase`, `align`, `resonate`, `underscore`, `highlight`, `emphasize`, `seamlessly`, `transformative`, `nuanced`, `multifaceted`, `compelling`

If the paragraph has more than 2–3 of these per 100 words, rewrite.

---

## 15. Type-Token Ratio check

Skim the document and notice whether the same words keep appearing. AI text has a lower type-token ratio than human text — it reuses vocabulary more.

**Check:** does the same adjective appear more than twice in 200 words? The same linking phrase? Replace repeats with direct statements or varied phrasing.

---

## 16. The reread

Read the entire document straight through, paying attention to whether you're learning anything in each sentence. If a sentence passes without imparting a fact, an argument, or a turn — cut it.

The output should usually be shorter after this pass than before, sometimes by 20–40%.

---

## Final yes/no questions

Before delivering, answer honestly:

1. Could each paragraph appear in an article about another subject with minor changes? If yes, that paragraph is too generic.
2. Is there any sentence that says "X is important" without explaining *how* X is important? Cut it.
3. Does every paragraph fall between 3–5 sentences? If yes, vary the lengths.
4. Is there even one fragment, one conjunction-starting sentence, or one contraction? If not and the context allows them, add some.
5. Is the emotional register exactly the same from start to finish? If yes, introduce variation.
6. Would a careful copy editor leave this prose alone, or would they cut a third of it? If the latter, do the cut now.

If the answer to any of 1–6 is uncomfortable, run the relevant pass again before delivering.
