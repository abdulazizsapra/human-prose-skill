# Patterns reference

Extended catalog of structural patterns with before/after examples. Load this file when:

- A first revision pass still reads as AI-generated
- The user wants concrete examples of what to change
- Working on long-form content with many patterns to address
- Teaching or explaining the patterns to someone else

Each section here pairs the pattern from the Wikipedia document with a concrete rewrite example.

---

## 1. Puffery / undue significance

### Pattern

Adding statements about how the subject represents or contributes to broader importance, especially in introductions and conclusions.

### Before

> The Statistical Institute of Catalonia was officially established in 1989, marking a pivotal moment in the evolution of regional statistics in Spain. The founding of Idescat represented a significant shift toward regional statistical independence, enabling Catalonia to develop a statistical system tailored to its unique socio-economic context. This initiative was part of a broader movement across Spain to decentralize administrative functions and enhance regional governance.

### After

> The Statistical Institute of Catalonia was established in 1989. It was created as part of Spain's post-Franco decentralization of administrative functions to the autonomous communities.

### Why

Three sentences in the original carry one fact (founding date, 1989) and one piece of context (Spanish decentralization). Everything else is empty significance signaling. The revision is roughly a third the length and carries more information per word.

### General rule

When the model would otherwise reach for "marking a pivotal moment," check whether the surrounding sentence has *any* specific fact. If not, the entire sentence is filler. Delete it.

---

## 2. Superficial analysis (participial tails)

### Pattern

Sentences end with comma + present-participle phrase asserting broader meaning.

### Before

> The station has 8 tracks and 6 platforms, serving as a major railway hub with historical significance. Historically, it has been crucial for linking Darbhanga with significant cities like Delhi, Patna, and Kolkata, facilitating the movement of passengers and goods.

### After

> The station has 8 tracks and 6 platforms. It connects Darbhanga to Delhi, Patna, and Kolkata.

### Why

"Serving as a major railway hub" is what having 8 tracks and 6 platforms *means*. "Facilitating the movement of passengers and goods" is what a railway *does*. The revisions cut the tautologies.

### Test

Read each sentence backwards from its last comma. If the part after the comma is a present participle and could be deleted without losing any fact, delete it.

---

## 3. Notability advertising

### Pattern

Listing the outlets that have covered a subject, often with adjectival praise of the outlets.

### Before

> The subject has been profiled in multiple high-quality, independent, and widely-read outlets, including The Australian, SBS News, 7News, and coverage syndicated through the Associated Press—appearing in platforms like The Senior and Perth Now. These sources provide significant, substantial, secondary coverage, not trivial mentions or press releases.

### After

> She has been profiled in The Australian, on SBS News, and on 7News.

### Why

The adjective stack ("high-quality, independent, widely-read") and the meta-claim ("significant, substantial, secondary coverage, not trivial mentions") are arguing for the subject's notability *to the reader of the article*. That's not how encyclopedic prose works. State the facts; let the reader judge.

### Always cut

- "active social media presence" (and all variants)
- Lists framed as "including [list], among others"
- Adjective stacks describing media outlets

---

## 4. Vague attributions

### Pattern

Opinions or claims attributed to unnamed groups.

### Before

> Modern researchers treat Kwararafa as a fluid political and cultural formation rather than a fixed state.

### After (with one source)

> Smith (2008) treats Kwararafa as a fluid political and cultural formation rather than a fixed state.

### After (with no specific source)

> [Delete the sentence.]

### Pattern variants to avoid

- "scholars have noted"
- "researchers have observed"
- "experts argue"
- "observers have commented"
- "critics have suggested"
- "industry analysts believe"

Either name the person or organization, or cut the sentence. There is no third option.

---

## 5. The challenges/future template

### Pattern

Late-article paragraph asserting that the subject faces challenges but is well-positioned.

### Before

> Despite its industrial and residential prosperity, Korattur faces challenges typical of urban areas, including traffic congestion, water scarcity, and waste management. With its strategic location and ongoing initiatives, Korattur continues to thrive as an integral part of the Ambattur industrial zone, embodying the synergy between industry and residential living.

### After

> [Delete the paragraph entirely.]

### Or, if there's a real sourced point

> A 2022 municipal report found that Korattur's groundwater levels had fallen by 40% over the previous decade, prompting the city to begin restricting industrial water draws.

### Why

The "despite challenges...continues to thrive" structure is a content-free formal closing. It exists because LLMs default to ending sections with sentiment. Cut it. If a real challenge is worth describing, describe it specifically and in its own paragraph, not as a generic closing flourish.

---

## 6. Negative parallelisms

### Pattern A: "not just X, but Y"

#### Before

> Self-Portrait by Yayoi Kusama constitutes not only a work of self-representation, but a visual document of her obsessions, visual strategies and psychobiographical narratives.

#### After

> Self-Portrait works simultaneously as self-representation and as a document of Kusama's recurring obsessions.

### Pattern B: "it's not X, it's Y"

#### Before

> Through this lens, Kusama's self-portrait is not a mirror but a portal: not a representation of self, but a mechanism for its constant reinvention.

#### After

> Through this lens, the self-portrait functions less as a mirror than as a mechanism for self-reinvention.

### When to use the construction

The negative-parallelism structure works when the contrast is real and surprising — when readers would genuinely expect the first thing and need to be redirected. It fails when the contrast is manufactured ("not just a building, but a community") because no one actually thought it was just a building.

Use it at most once per long piece, and only on a contrast that earns the rhetorical weight.

---

## 7. Rule-of-three lists

### Pattern

Constructing lists of three items where two or four would be more natural.

### Before

> The temple's color palette of blue, green, and gold resonates with the region's natural beauty, symbolizing Texas bluebonnets, the Gulf of Mexico, and the diverse Texan landscapes.

### After

> The blue, green, and gold color palette refers to local landscape: bluebonnets and the Gulf coast.

### Why

The first version uses three colors symbolizing three things (a 3x3). The second keeps the colors (which are factual) and reduces the symbolism to two items (which are specific). The "diverse Texan landscapes" is filler — it just means "Texas."

### Practice

Count parallel items in your prose. If three keeps appearing — three adjectives, three nouns, three clauses — break it up. Use one. Use two. Use four. Vary.

---

## 8. Copula avoidance

### Pattern

Replacing plain "is" / "has" with marketing verbs.

### Before

> Gallery 825 on La Cienega Boulevard serves as LAAA's exhibition space for contemporary art. The gallery features four separate spaces.

### After

> Gallery 825 on La Cienega Boulevard is LAAA's contemporary-art exhibition space. It has four rooms.

### Substitution list

| AI form | Plain form |
| --- | --- |
| serves as | is |
| stands as | is, was |
| acts as | is |
| represents | is |
| constitutes | is |
| functions as | is |
| operates as | is |
| boasts | has |
| features | has |
| offers | has, provides |
| holds the distinction of being | is, was |

---

## 9. The "refers to" lead

### Pattern

Opening encyclopedic articles by treating the title as a phrase being defined.

### Before

> "EuroGames editions" is the chronological list of the biennial EuroGames, a European LGBT+ multi-sport event organized by the European Gay and Lesbian Sport Federation.

### After

> The EuroGames are a biennial European LGBT+ multi-sport event organized by the European Gay and Lesbian Sport Federation. This article lists the editions chronologically.

### Why

The original treats the list title as if it were an object in the world. It isn't — it's the article's filing label. Lead with the subject; mention the article's structure separately if needed.

---

## 10. Knowledge-cutoff hedging

### Pattern

Acknowledging lack of information, then speculating.

### Before

> While specific information about the fauna of Studniční hora is limited in the provided search results, the mountain likely supports populations of small mammals, birds adapted to subalpine conditions, and various invertebrate species common to the region.

### After

> [Delete entirely.]

### Why

Every clause after "limited" is speculation. The sentence is the model bridging a knowledge gap with plausible-sounding generic content. None of it is sourced; none of it should be in the output.

### Rule

If a sentence's premise is "X isn't well documented, but...," the rest of the sentence is invented. Delete the whole sentence. Do not try to rescue it.

---

## 11. Section summaries / conclusions

### Pattern

Ending sections or articles with a sentence that restates what was just said.

### Before

> In summary, the educational and training trajectory for nurse scientists typically involves a progression from a master's degree in nursing to a Doctor of Philosophy in Nursing, followed by postdoctoral training in nursing research. This structured pathway ensures that nurse scientists acquire the necessary knowledge and skills to engage in rigorous research and contribute meaningfully to the advancement of nursing science.

### After

> [Delete entirely. The preceding section already said this.]

### Why

The reader has the information. Restating it patronizes them. Real articles end when their last specific fact ends. They don't have outros.

---

## 12. Inline-header bullet lists

### Pattern

Bulleted lists where every item is bold-header-colon-explanation.

### Before

> **Standard Rotary Saws:** Typically used for drywall and light materials.
> **Heavy-Duty Rotary Saws:** Designed for tougher materials such as tiles, metals, and plastics.
> **Corded and Cordless Versions:** Corded rotary saws offer continuous power, while cordless versions provide portability and convenience.

### After (option 1: prose)

> Standard rotary saws handle drywall and light materials, while heavy-duty versions cut tile and metal. Both come in corded and cordless versions; corded models run continuously, cordless ones are easier to move around.

### After (option 2: plain bullets)

> - Standard rotary saws cut drywall and light materials.
> - Heavy-duty rotary saws cut tile, metal, and plastic.
> - Corded models run continuously; cordless models are portable.

### Why

The inline-header pattern is a tell because it's borrowed from slide decks, marketing one-pagers, and AI chat output. Encyclopedic and analytical writing uses either prose or plain bullets — almost never inline-headered bullets.

---

## 13. Em-dash overuse

### Pattern

Reaching for em dashes to "punch up" sentences.

### Before

> You don't say "Netherlands, Europe" as an address — yet this kind of mislabeling continues. The term is primarily promoted by Dutch institutions — not by the people of the autonomous countries themselves — even placing it in addresses, e.g., "Curaçao, Dutch Caribbean."

### After

> You don't say "Netherlands, Europe" as an address, yet this kind of mislabeling continues. The term is promoted primarily by Dutch institutions, not by the people of the autonomous countries themselves. It even appears in addresses (e.g., "Curaçao, Dutch Caribbean").

### Rule of thumb

In a 500-word piece, expect 0–2 em dashes from a careful human writer. If your draft has more than that, audit them. Most will resolve to commas, parentheses, or sentence breaks.

---

## 14. Heading style

### Pattern A: title case

#### Before

> ## Impact of Technology and Digitalization
> ## Sustainable Development and Environmental Law
> ## Human Rights and Economic Law

#### After

> ## Impact of technology and digitalization
> ## Sustainable development and environmental law
> ## Human rights and economic law

### Pattern B: skipping heading levels

If the document starts with `#`, the next heading should be `##`, not `###`. Don't skip. The Wikipedia document specifically calls out skipping `##` and going straight to `###` as a Markdown-import tell.

### Pattern C: thematic breaks before headings

Don't insert `---` before every heading. Headings introduce their own breaks. Thematic breaks should be rare and meaningful.

---

## 15. Phrasal templates with un-filled placeholders

### Pattern

Pasting LLM output that still contains `[INSERT NAME HERE]`-style placeholders.

### Examples to watch for

- `[Your Name]`
- `[Insert link to source]`
- `[Describe the specific section]`
- `[link to article]`
- `2025-XX-XX` in access-date fields
- `PASTE_YOUTUBE_VIDEO_URL_HERE`
- `URL` as a literal placeholder
- `[overgen 1]` (referee markup leak)

### Rule

Before delivering any output, search for `[`, `XX`, `INSERT`, `PASTE`, `HERE`. Any match is an unfilled placeholder. Either fill it or remove the surrounding text.

---

## 16. UI-leakage artifacts

### Pattern

Strings from the chatbot interface that should never appear in pasted output.

### Examples

- `utm_source=chatgpt.com`
- `utm_source=openai`
- `utm_source=copilot.com`
- `referrer=grok.com`
- `citeturn0search0` (and similar `turn0...` patterns)
- `:contentReference[oaicite:N]{index=N}`
- `oai_citation:N‡domain.com`
- `【85†L261-269】`
- `[attached_file:N]` / `[web:N]`
- `<grok-card data-id="...">`
- `grok_render_citation_card_json={"cardIds":[...]}`
- `({"attribution":{"attributableIndex":"X-Y"}})`
- ✓ ✗ ↩ as inline glyphs in references

### Rule

Audit any URL pasted as a citation for tracking parameters. Audit any reference list for non-standard glyphs and bracketed numeric tags. Strip all of them.

---

## 17. Emoji as formatting

### Pattern

Using emoji as section markers or bullet decorations.

### Before

> 🧠 **Cognitive Dissonance Pattern**
> 🧱 **Structural Gatekeeping**
> 🚨 **Underlying Motivation**

### After

> ## Cognitive dissonance
> ## Structural gatekeeping
> ## Motivation

### Rule

No emoji in formal prose unless the user has explicitly indicated they want a casual register where emoji are normal (e.g., a Slack post, a tweet). Even then, use them sparingly.

---

## 18. Promotional tone in biography

### Pattern

Writing about people as if pitching them.

### Before

> CEO Allan Kilavuka emphasized the airline's commitment to sustainability, customer focus, and Africa's prosperity through responsible corporate practices.

### After

> In a November 2024 statement, Kilavuka said the airline was prioritizing emissions reductions, customer service improvements, and African development.

### Or, if you don't have a source

> [Delete the sentence.]

### Why

The first version is corporate PR. It has three abstractions ("sustainability," "customer focus," "Africa's prosperity") and one buzzword cluster ("responsible corporate practices"). The second version names the action (a statement) and gives the date. If you can't name those, you're not reporting; you're advertising.

---

## 19. The travel-brochure opening

### Pattern

Article openings that read like guidebook copy.

### Before

> Nestled within the breathtaking region of Gonder in Ethiopia, Alamata Raya Kobo stands as a vibrant town with a rich cultural heritage and a significant place within the Amhara region. From its scenic landscapes to its historical landmarks, Alamata Raya Kobo offers visitors a fascinating glimpse into the diverse tapestry of Ethiopia.

### After

> Alamata is a town in the Amhara Region of northern Ethiopia. As of the 2007 census it had a population of approximately 33,000.

### Why

The original has zero factual content. It's six clauses of atmosphere. The revision says where the town is and how big it is. That's what an encyclopedia opening should do.

### Rule

If an opening paragraph contains words from the travel-brochure list (`nestled`, `breathtaking`, `vibrant`, `charming`, `picturesque`, `offers visitors`, `fascinating glimpse`), rewrite the entire paragraph from facts.

---

## 20. The press-release voice

### Pattern

Articles about products or companies that read like the marketing copy.

### Before

> The SOLLEI's exterior design communicates a powerful emotional presence, staying true to Cadillac's signature bold proportions. Its low, elongated silhouette is highlighted by a wide stance and an extended coupe door, which enhances accessibility to the spacious rear cabin. Smooth, uninterrupted surfaces and a pronounced A-line accentuate the vehicle's overall length, while a sleek, low tail imparts a sense of refined dynamism.

### After

> The Sollei is a two-door coupe convertible. Cadillac describes its styling as a return to the brand's mid-century proportions; the body has no traditional door handles, using flush buttons instead.

### Why

The original is the press release verbatim. The revision keeps the actual facts (two-door coupe, no traditional handles) and attributes the brand-positioning claim to Cadillac rather than asserting it as fact.

### Rule

If a passage reads like ad copy, identify which sentences contain verifiable facts and which contain only sentiment. Keep the first kind, possibly with attribution. Delete the second kind.
