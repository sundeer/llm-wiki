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
Philosophers, ideologues, theorists, and politicians. Cover identity, intellectual lineage, key ideas, and influence on or adoption by the New Right.
Examples: Carl Schmitt, Leo Strauss, Patrick Deneen, Curtis Yarvin, J.D. Vance, Steve Bannon

### Movements (`Wiki/Movements/<Name>.md`)
Ideological and political movements that make up or feed into the New Right. Cover what it is, when it emerged, who leads it, core beliefs, and relationship to other movements and to MAGA.
Examples: National Conservatism, Christian Nationalism, Paleoconservatism, Integralism, Post-liberalism

### Concepts (`Wiki/Concepts/<Name>.md`)
Political philosophy and political theory terms central to understanding the New Right. Cover definition, intellectual origin, how the New Right uses or adapts it, and relationship to other concepts.
Examples: Decisionism, Illiberalism, Populism, Sovereigntism, Administrative State, Natural Law

### Texts (`Wiki/Texts/<Title>.md`)
Books, papers, essays, and articles — primary or secondary sources. Cover author, year, genre (book / essay / article), core argument and key claims, relation to the New Right thesis, and contradictions or tensions with other texts in the wiki.

### Events (`Wiki/Events/<Name>.md`)
Historical events that shaped the New Right's development. Cover date, actors, what happened, and significance for the conservative movement.
Examples: 2016 election, January 6 2021, Tea Party rise, Pat Buchanan's 1992 "Culture War" speech

### Institutions (`Wiki/Institutions/<Name>.md`)
Think tanks, media outlets, organizations, and networks. Cover founding, mission, key figures, and role in developing or amplifying New Right ideas.
Examples: Claremont Institute, Heritage Foundation, American Greatness, First Things

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

Navigation map; LLM-maintained. Read first when answering queries. Update on every ingest. See `index.md` itself for the format.

---

## log.md

Append-only operation log. Operations: `ingest`, `query`, `synthesis`, `lint`. See `log.md` for the entry format. Recent entries: `grep "^## \[" log.md | tail -10`.

---

## Operations

The four core workflows live as skills under `.claude/skills/`. Invoke explicitly with `/ingest`, `/query`, `/synthesis`, `/lint`, or describe the task in natural language and the matching skill triggers from its description. Skill bodies contain the step-by-step procedures previously inlined here.

---

## Tone and Style

- Write for a reader who is intelligent but new to conservative political theory
- Explain jargon on first use; link to the Concepts page for recurring terms
- Be precise about the difference between a thinker's *original* ideas and how those ideas are *used* by the New Right (the two often differ significantly)
- Flag contested or disputed claims as such
- Prefer synthesis over mere summary — the wiki should develop a thesis, not just catalog facts
