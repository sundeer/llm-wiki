# LLM Wiki Schema

## Purpose

This wiki is a persistent, compounding research knowledge base on the transformation of American conservatism into the MAGA New Right. It synthesizes political philosophy, political theory, historical roots, key thinkers, and movements. The anchor text is *Furious Minds* by Laura K. Field.

The LLM writes and maintains the wiki. The human curates sources, directs analysis, and asks questions.

---

## Directory Structure

```
llm-wiki/
├── CLAUDE.md          ← this file (schema + conventions)
├── index.md           ← content catalog (LLM-maintained)
├── log.md             ← append-only operation log (LLM-maintained)
├── Clippings/         ← raw sources: web clippings (immutable)
├── Raw/               ← raw sources: PDFs, transcripts, other files (immutable)
└── Wiki/              ← LLM-generated wiki pages
    ├── Overview.md
    ├── Inbox/         ← uncategorized stubs (Obsidian default landing zone)
    ├── Thinkers/
    ├── Movements/
    ├── Concepts/
    ├── Texts/
    ├── Events/
    └── Institutions/
```

**Raw sources are immutable.** The LLM reads them but never modifies them. All generated content lives in `Wiki/`.

---

## Page Types

### Thinkers (`Wiki/Thinkers/<Name>.md`)
Philosophers, ideologues, political theorists, and politicians relevant to the New Right.
- Who they are, intellectual lineage, key ideas
- Influence on or adoption by the MAGA New Right
- Relationship to other thinkers and movements
- Examples: Carl Schmitt, Leo Strauss, Patrick Deneen, Curtis Yarvin, J.D. Vance, Steve Bannon

### Movements (`Wiki/Movements/<Name>.md`)
Ideological and political movements that make up or feed into the New Right.
- What it is, when it emerged, who leads it
- Core beliefs and policy agenda
- Relationship to other movements and to MAGA
- Examples: National Conservatism, Christian Nationalism, Paleoconservatism, Integralism, Post-liberalism

### Concepts (`Wiki/Concepts/<Name>.md`)
Political philosophy and political theory terms central to understanding the New Right.
- Definition and intellectual origin
- How it is used or adapted by the New Right
- Relationship to other concepts
- Examples: Decisionism, Illiberalism, Populism, Sovereigntism, Administrative State, Natural Law

### Texts (`Wiki/Texts/<Title>.md`)
Books, papers, essays, and articles that are primary or secondary sources.
- Author, year, genre (book / essay / article)
- Core argument and key claims
- How it relates to the New Right thesis
- Contradictions or tensions with other texts in the wiki

### Events (`Wiki/Events/<Name>.md`)
Historical events that shaped the New Right's development.
- Date, actors, what happened
- Significance for the conservative movement
- Examples: 2016 election, January 6 2021, Tea Party rise, Pat Buchanan's 1992 "Culture War" speech

### Institutions (`Wiki/Institutions/<Name>.md`)
Think tanks, media outlets, organizations, and networks.
- Founded, mission, key figures
- Role in developing or amplifying New Right ideas
- Examples: Claremont Institute, Heritage Foundation, American Greatness, First Things

---

## Frontmatter (all pages)

```yaml
---
title: <page title>
type: <thinker|movement|concept|text|event|institution|overview>
tags: []
sources: []        # filenames of raw sources that contributed to this page
updated: YYYY-MM-DD
---
```

---

## Cross-Referencing

- Use Obsidian wikilinks: `[[Page Name]]`
- Always link to existing pages when mentioning known entities
- If a referenced entity has no page yet, create a stub with frontmatter and a one-line description
- Stubs are flagged with `tags: [stub]`

### Inbox (`Wiki/Inbox/`)

Obsidian is configured to create new files in `Wiki/Inbox/` when the user clicks an unresolved wikilink in the editor. Files that land here are **uncategorized placeholders** — they have no frontmatter and no content.

During a lint pass, the LLM must:
1. `find Wiki/Inbox/ -name "*.md"` to surface any new arrivals
2. For each file: determine its correct type (Thinker, Concept, Institution, etc.)
3. Move it to the right subdirectory and add frontmatter + a one-line stub description
4. Add it to `index.md`

Do not leave files in `Wiki/Inbox/` — it is a transit zone, not a permanent home.

---

## index.md

The index is the LLM's navigation map. Updated on every ingest.

Structure:
```
## Overview
- [[Overview]] — master synthesis of the wiki

## Thinkers
- [[Carl Schmitt]] — German jurist; source of decisionist theory adopted by the New Right

## Movements
...

## Concepts
...

## Texts
...

## Events
...

## Institutions
...
```

When answering a query, the LLM reads `index.md` first to identify relevant pages, then drills into them.

---

## log.md

Append-only chronological record. Each entry format:

```
## [YYYY-MM-DD] <operation> | <title>
<one-line summary>
Pages created: ...
Pages updated: ...
```

Operations: `ingest`, `query`, `synthesis`, `lint`

Parseable with: `grep "^## \[" log.md | tail -10`

---

## Operations

### Ingest
When the user adds a new source to `Clippings/` or `Raw/`:
1. Read the source in full
2. Discuss key takeaways with the user
3. Create or update a `Texts/` page for the source
4. Create or update all Thinker, Movement, Concept, Event, Institution pages touched by the source
5. Note explicitly where the source contradicts or revises existing wiki content
6. Update `index.md` and append to `log.md`
7. **Assess whether the source materially revises the Overview thesis.** Update `Overview.md` only if the source: (a) changes the arc's argument in a section that already exists, (b) introduces a major new thread the current sections don't account for, or (c) surfaces a significant contradiction with the existing synthesis. Most ingests will not require an Overview update — absorb the detail into individual pages and leave the Overview alone.

A single source typically touches 5–15 wiki pages.

### Query
When the user asks a question:
1. Read `index.md` to identify relevant pages
2. Read the relevant pages
3. Synthesize an answer with `[[wikilink]]` citations
4. Offer to file the answer as a new wiki page if it represents lasting synthesis

### Synthesis
When a query answer, discussion, or ingest produces a new or revised understanding of the arc:
1. Update `Overview.md` — revise the relevant section(s) of the narrative, or add a new section if a genuinely new thread emerges; do not append; rewrite the section to absorb the new insight
2. Update any individual pages whose cross-references or arguments need adjustment
3. Append to `log.md` with operation `synthesis`
4. The Overview's seven-section structure is the stable skeleton — new material should be absorbed into existing sections unless it truly requires a new one

### Lint
Periodic health check (ask the LLM to run this explicitly):
- **Check `Wiki/Inbox/`** for uncategorized files and resolve them first (see Cross-Referencing above)
- Flag contradictions between pages
- Flag stubs needing expansion
- Flag orphan pages (no inbound links)
- Flag concepts or people mentioned but lacking their own page
- Flag stale claims superseded by newer sources
- Suggest new sources or questions to investigate

---

## Tone and Style

- Write for a reader who is intelligent but new to conservative political theory
- Explain jargon on first use; link to the Concepts page for recurring terms
- Be precise about the difference between a thinker's *original* ideas and how those ideas are *used* by the New Right (the two often differ significantly)
- Flag contested or disputed claims as such
- Prefer synthesis over mere summary — the wiki should develop a thesis, not just catalog facts
