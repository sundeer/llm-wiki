---
name: query
description: Answer a question about the wiki's subject matter (American conservatism, the New Right, MAGA, named thinkers / movements / concepts / texts / events / institutions) by reading `index.md` first, then drilling into relevant pages, then synthesizing with `[[wikilink]]` citations. Triggers on substantive questions about the wiki's domain.
---

When the user asks a question:
1. Read `index.md` to identify relevant pages
2. Read the relevant pages
3. Synthesize an answer with `[[wikilink]]` citations
4. File the answer in `QA/` as a new entry:
   - Choose a short, descriptive topic name (e.g., `Liberal Neutrality Critique.md`)
   - Use this frontmatter:
     ```yaml
     ---
     title: <topic name>
     type: qa
     asked: YYYY-MM-DD
     wiki_sources:
       - Wiki/path/to/page.md
     ---
     ```
   - Structure the file as: question, then the full answer with `[[wikilink]]` citations, then a "Wiki Pages Consulted" list at the bottom
   - Add a row to `QA/index.md` with the entry title, date, and topic tags
