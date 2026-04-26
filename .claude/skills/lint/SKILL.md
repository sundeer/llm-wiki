---
name: lint
description: Run a wiki health check: resolve `Wiki/Inbox/` files first, then flag contradictions, stubs needing expansion, orphan pages, missing pages for entities mentioned elsewhere, and stale claims. Triggers on `/lint`, 'do a lint pass', 'health check the wiki', or similar.
---

Periodic health check (ask the LLM to run this explicitly):
- **Check `Wiki/Inbox/`** for uncategorized files and resolve them first (see Cross-Referencing in `CLAUDE.md`)
- Flag contradictions between pages
- Flag stubs needing expansion
- Flag orphan pages (no inbound links)
- Flag concepts or people mentioned but lacking their own page
- Flag stale claims superseded by newer sources
- Suggest new sources or questions to investigate
