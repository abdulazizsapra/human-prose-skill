# Human Prose — Claude Code Skill

A Claude Code skill that makes AI-generated prose read like a human wrote it. Drop it into any Claude Code project and it automatically applies when writing articles, blog posts, essays, biographies, reports, or any substantial prose output.

## What it does

LLMs default to a recognizable style: inflated significance claims, hollow filler phrases, reflexive rule-of-threes, participial tails, and a vocabulary full of words like *delve*, *tapestry*, *underscore*, and *robust*. These patterns aren't just AI-detector tells — they make writing feel padded and lifeless to any attentive reader.

This skill targets those patterns directly. It instructs Claude to:

- Cut puffery ("stands as a testament to", "plays a pivotal role") instead of rewriting it
- Replace generic claims with specific facts, or leave a gap rather than inventing filler
- Use plain verbs ("is", "has", "was") instead of marketing substitutes ("serves as", "boasts", "showcases")
- Vary sentence and list structure rather than defaulting to threes
- Avoid weasel attributions ("experts argue", "observers note") unless a real source is named
- Never pad around missing information with hedges like "based on available information..."
- Strip Markdown artifacts, hallucinated citations, and discussion-page contamination

The core principle: **specific beats generic, always**. If a sentence could appear in an article about almost any other subject in the same category, it's failing.

## Files

```
SKILL.md              — Main skill definition (what Claude reads)
human-prose.skill     — Packaged skill file for direct installation
checklist.md          — Pre-publish search-and-cut checklist
patterns.md           — Extended pattern catalog with before/after examples
vocabulary.md         — Full word list organized by LLM era, with substitutions
```

## Installation

### Option 1: Use the packaged skill file

Copy `human-prose.skill` into your Claude Code project's `.claude/skills/` directory (create the directory if it doesn't exist):

```bash
mkdir -p .claude/skills
cp human-prose.skill .claude/skills/
```

### Option 2: Use the raw SKILL.md

Copy `SKILL.md` into `.claude/skills/human-prose/SKILL.md` in your project:

```bash
mkdir -p .claude/skills/human-prose
cp SKILL.md .claude/skills/human-prose/SKILL.md
```

The skill activates automatically when you write prose through Claude Code. You can also invoke it explicitly by asking Claude to "humanize" existing text.

## When it triggers

Claude Code loads this skill any time prose output exceeds a few sentences — articles, blog posts, encyclopedia entries, biographies, reports, rewrites, or any "humanize this" request. You don't need to invoke it explicitly; it applies to all substantial written content.

## The reference files

Three companion files support deeper revision work:

- **`checklist.md`** — A fast search-and-cut pass to run before publishing. Lists the highest-priority strings to find and remove.
- **`patterns.md`** — Extended before/after examples for every major pattern category.
- **`vocabulary.md`** — Full word catalog organized by LLM era (GPT-4 through mid-2025 models), so you can identify which generation of tells a piece is showing.

The main `SKILL.md` handles routine prose generation. Load the references when revising long documents or when a first pass still reads formulaic.

## Humanizing existing AI text

Ask Claude: *"humanize this"* and paste your text. The skill applies this sequence:

1. Cut puffery sentences entirely — don't rewrite, delete
2. Replace generic claims with specifics only when the facts are actually known
3. Break up rule-of-three lists into pairs, singles, or longer runs
4. Swap fancy verbs for plain ones
5. Vary sentence length deliberately
6. Audit and reduce em dashes, bold text, and heading depth
7. Re-read the whole piece — if it still sounds like a model generating what an article should look like, cut more

The output of a humanize pass is almost always shorter than the input. Same length usually means the job isn't done.

## License

MIT
