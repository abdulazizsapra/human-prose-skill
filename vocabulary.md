# Vocabulary reference

Full catalog of words and phrases that LLMs overuse. Load this file when:

- Revising long-form content for AI tells
- The user reports that a previous output still "sounds AI"
- Doing a final pass on a piece that will be published or submitted somewhere AI-skeptical
- The user specifically asks about which words to avoid

## How to use this file

Words below are organized by the LLM "era" in which they were most prominent. This matters because frequency has shifted: `delve` was famously overused in 2023–2024 and is now suppressed in many newer models, while `emphasizing`, `highlighting`, and `showcasing` have become the new tells. A piece using only mid-2025-era words can still read as AI to a current reader.

For each word, the rule is the same: **one in passing is fine; clusters are a problem**. The fix is usually deletion or a plainer substitute, not a fancier synonym.

---

## Tier 0: statistically extreme outliers (100x+ human frequency)

Research using Douglas Biber's lexical feature analysis (PNAS, 2024) measured specific words in instruction-tuned AI output vs. human text. These appear at astronomical multiples of human frequency — introduced by the RLHF instruction-tuning process, not base model pre-training. Treat these as immediate disqualifiers: one use flags the entire passage.

| Word | Multiple above human frequency | Rule |
| --- | --- | --- |
| camaraderie | 147–171× | Never use. No exceptions. |
| tapestry (figurative) | 147–155× | Delete. Every time. |
| intricate / intricacies | 119–129× | Replace with "complex" or name the specific detail |
| palpable | 95–145× | Replace with a concrete sensory description |
| amidst | 90–100× | Use "amid" or "in" |
| testament (figurative) | documented | Delete. Every time. |
| vibrant | documented | Cut, or describe what's actually happening |
| delve / delving | documented | Use "examine," "look at," "study" |

---

## Tier 1: high-priority avoid list (current era)

These appear constantly in current AI output. Cut or replace aggressively.

| Word / phrase | Plainer substitute (or: cut) |
| --- | --- |
| emphasizing | showing, stressing — usually cut |
| highlighting | showing — usually cut |
| showcasing | showing, displaying — usually cut |
| enhance / enhances | improve, increase, add to |
| underscore (verb) | show, suggest — usually cut |
| crucial | important, central — often cut |
| pivotal | important, decisive — often cut |
| key (as adjective) | main, important — often cut |
| robust | strong, well-built, durable |
| navigate (figurative) | handle, work through, deal with |
| foster / fostering | encourage, build, support |
| valuable insights | (cut, replace with what was learned) |
| align with / aligns with | match, fit, accord with |
| resonate with | matter to, ring true for |
| ensure / ensuring | make sure, see that |
| reflect / reflecting (broader) | (cut the broader claim) |
| contribute to / contributing to | (cut the participial tail) |
| serve as / serves as | is, was, acts as |
| stand as / stands as | is, was |
| seamlessly | (cut — nothing is ever seamless) |
| transformative | (cut — specify what changed) |
| multifaceted | (cut — say what the facets are) |
| nuanced | (cut — say what the nuance is) |
| groundbreaking | (cut — say why it's new) |
| innovative | (cut — say what's new about it) |
| compelling | (cut — either argue the case or don't) |

## Tier 2: 2023–2024 (GPT-4) tells

These dropped off in newer models but appear in older pasted content. Heavy revision triggers.

| Word / phrase | Substitute |
| --- | --- |
| delve / delving into | examine, study, look at |
| tapestry (figurative) | (cut entirely) |
| testament (figurative) | (cut entirely) |
| boast / boasts (figurative) | has |
| bolster / bolstered | strengthen, support |
| meticulous / meticulously | careful, carefully |
| intricate / intricacies | complex, complexity, detail |
| garner / garnered | receive, earn, get |
| interplay | interaction — or cut |
| landscape (abstract noun) | field, area, scene — or cut |
| Additionally (sentence-initial) | Also, And — or cut |
| Notably (sentence-initial) | (often just cut) |
| Consequently (sentence-initial) | So, Thus, As a result |
| Furthermore | Also, And |
| Moreover | Also |
| In essence | (cut) |
| Ultimately | (often cut) |
| At its core | (cut) |
| At the heart of | (cut, name the thing directly) |
| In the realm of | In, Within |
| In the world of | In |

## Tier 3: significance and importance signaling

Whole phrases that flag inflated importance. Treat the whole phrase as the unit to delete.

- "stands as a testament to"
- "serves as a testament to"
- "is a testament to"
- "leaves an indelible mark"
- "leaves a lasting impression"
- "carries a profound legacy"
- "shaping the [anything]"
- "shapes the future of"
- "marks a turning point"
- "marks a significant shift"
- "represents a watershed moment"
- "key turning point"
- "evolving landscape"
- "focal point of"
- "rich cultural heritage"
- "rich tapestry of"
- "diverse tapestry"
- "vibrant community"
- "vibrant culture"
- "vibrant ecosystem"
- "deeply rooted in"
- "deeply ingrained"
- "central to the identity"
- "an integral part of"
- "plays a pivotal role"
- "plays a crucial role"
- "plays a vital role"
- "plays a key role"
- "plays a significant role"
- "plays an important role"
- "broader implications for"
- "broader context of"
- "wider movement"
- "larger conversation about"
- "ongoing discourse"
- "contemporary discussion"
- "speaks to the broader"

## Tier 4: notability and source-laundering phrases

These appear when AI tries to assert that a subject is important by gesturing at coverage.

- "independent coverage"
- "widely covered in"
- "featured in [list of outlets]"
- "profiled in"
- "received attention from"
- "garnered attention"
- "media attention"
- "active social media presence"
- "strong digital presence"
- "growing online following"
- "written by a leading expert"
- "leading authority in the field"
- "recognized expert"
- "internationally recognized"
- "widely respected"
- "well-regarded"
- "highly regarded"

## Tier 5: travel-brochure / brochure-speak

When the topic is a place, a building, a product, or a cultural item:

- "nestled in / nestled among / nestled within"
- "in the heart of"
- "tucked away in"
- "set against the backdrop of"
- "boasts breathtaking views"
- "breathtaking landscapes"
- "scenic vistas"
- "stunning natural beauty"
- "picturesque"
- "charming"
- "quaint"
- "bustling"
- "captivating"
- "enchanting"
- "a fascinating glimpse into"
- "offers visitors"
- "invites visitors to"
- "a true gem"
- "a hidden gem"
- "a must-visit"

## Tier 6: hedges and gap-fillers

These appear when the model doesn't have the information and is bridging the gap.

- "While specific details are limited / scarce / not widely documented..."
- "Information about X is not extensively documented..."
- "Based on available information..."
- "As of my last knowledge update..."
- "Up to my training data..."
- "In the absence of [specific records / detailed sources]..."
- "[Subject] maintains a low profile"
- "[Subject] keeps personal details private"
- "[Subject] prefers to stay out of the public eye"
- "Little is publicly known, though..."
- "While not extensively covered, it is believed that..."

**Rule:** if a sentence starts with any of these, the entire sentence is almost certainly speculation. Delete it. Do not rewrite.

## Tier 7: superficial-analysis participial tails

Cut the participial phrase. Sometimes cut the whole sentence. Note: **any** present participial clause, not just these specific phrases, is a detection signal at above-human rates. Audit all of them.

- "...contributing to the [region's / community's / industry's] [growth / development / character]"
- "...cementing its status as..."
- "...solidifying its role as..."
- "...reinforcing its position as..."
- "...reflecting [broader / wider / ongoing] [trends / movements / shifts]"
- "...symbolizing [unity / progress / heritage]"
- "...embodying the spirit of..."
- "...echoing through generations"
- "...resonating with audiences"
- "...capturing the imagination of..."
- "...inspiring a new generation"
- "...paving the way for..."
- "...setting the stage for..."
- "...laying the groundwork for..."
- "...heralding a new era of..."

## Tier 8: meta-commentary in talk / discussion contexts

If the writing is a comment, reply, or message, never use:

- "I hope this helps"
- "Let me know if you have questions"
- "Please don't hesitate to..."
- "I am committed to..."
- "I assure you that..."
- "My goal is to ensure..."
- "I am open to feedback"
- "I welcome any guidance"
- "Thank you for your consideration"
- "I look forward to..."
- "Of course!" / "Certainly!" / "Absolutely!"
- "You're absolutely right!"
- "Great question!"
- "Here's a [breakdown / overview / summary]..."
- "Below is..."
- "I'd be happy to..."

## Tier 9: structural framing phrases

- "It is [important / worth / crucial / vital] to note that..."
- "It is worth mentioning that..."
- "It should be noted that..."
- "One thing to keep in mind is..."
- "It is interesting to note..."
- "Interestingly..."
- "Notably..."
- "Of particular note..."
- "What's more..."
- "That said..."

These are almost always cuttable. Just state the next thing.

## Tier 10: certainty and causal overuse

AI-generated text shows 111–152% more certainty markers than human text, and 50–67% more causal expressions than human text in factual writing.

**Certainty markers to audit:**

- "clearly"
- "obviously"
- "certainly"
- "is fundamental"
- "is essential"
- "undeniably"
- "without question"
- "it is clear that"
- "there is no doubt that"

**Causal over-connectors:**

- "therefore"
- "consequently"
- "as a result"
- "thus"
- "hence"

One of these in a document is fine. When they appear every few sentences, the causal-density pattern is itself a tell. Replace most with no connector at all — let the logic flow without announcing it.

---

## Co-occurrence patterns

Finding one of these should trigger a document-wide search, not just a local fix:

- **GPT-4 cluster:** delve + intricate + tapestry + testament + vibrant + meticulous + crucial + pivotal + underscore
- **GPT-4o cluster:** align with + foster + enhance + showcase + crucial + pivotal + enduring + vibrant + underscore
- **GPT-5 / Claude cluster:** emphasizing + highlighting + showcasing + enhance (often alongside notability claims and lists of media outlets)
- **Tier-0 cluster:** palpable + amidst + camaraderie + tapestry + intricate — seeing two of these together is a strong signal; seeing three is definitive

---

## The deletion rule

For most words in this file, the right answer is not to substitute a synonym but to delete the word and see if the sentence still works. It usually does, and is usually better for the loss.

When a sentence breaks under deletion, the question is whether the *idea* the word was carrying is one you have evidence for. If yes, rewrite the sentence around the concrete evidence. If no, delete the sentence too.

---

## Words that should appear *more* in human-like prose

Research identifies what's *absent* from AI text, not just what's present. Human prose uses more:

- **Contractions**: it's, don't, we've, can't, they're, won't, I'd, you'll
- **Sentence-initial conjunctions**: "But," "And," "So," "Yet," "Or"
- **Direct address**: "you," "your" used in the reader-address sense
- **First-person perspective**: "I think," "in my view," "what I found" — when the context is appropriate
- **Specific proper nouns**: names, dates, places, numbers — not "some researchers" or "a recent study"
- **Informal or colloquial expressions** — calibrated to context; not forced
- **Questions** — rhetorical, direct, or exploratory
- **Fragment sentences** — for rhetorical emphasis
- **Passive voice** — counterintuitively, humans use more passive than AI; use it where it fits naturally
