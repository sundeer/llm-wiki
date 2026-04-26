---
name: ingest
description: Process a new source the user has added to `Clippings/` or `raw/`. Triggers when the user says they've added a clipping, PDF, transcript, article, or asks to ingest / process / read in / work through a new source. Creates a `Texts/` page and updates all touched Thinker / Movement / Concept / Event / Institution pages, plus `index.md` and `log.md`.
---

When the user adds a new source to `Clippings/` or `Raw/`:
1. Read the source in full
2. Discuss key takeaways with the user
3. Create or update a `Texts/` page for the source
4. Create or update all Thinker, Movement, Concept, Event, Institution pages touched by the source
5. Note explicitly where the source contradicts or revises existing wiki content
6. Update `index.md` and append to `log.md`
7. **Assess whether the source materially revises the Overview thesis.** Update `Overview.md` only if the source: (a) changes the arc's argument in a section that already exists, (b) introduces a major new thread the current sections don't account for, or (c) surfaces a significant contradiction with the existing synthesis. Most ingests will not require an Overview update — absorb the detail into individual pages and leave the Overview alone.

A single source typically touches 5–15 wiki pages.
