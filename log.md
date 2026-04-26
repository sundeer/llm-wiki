# Wiki Log

*Append-only record of all wiki operations. Format: `## [YYYY-MM-DD] <operation> | <title>`*
*Quick parse: `grep "^## \[" log.md | tail -10`*

---

## [2026-04-25] init | Wiki scaffolding created
Initial directory structure, CLAUDE.md schema, index.md, and log.md created.
Pages created: Overview.md (stub)
Pages updated: —

## [2026-04-26] ingest | Furious Minds pp. 1–300 (Chapters 1–10 complete, Chapter 11 begun)
Systematic ingest of *Furious Minds* by Laura K. Field (Princeton UP, 2025), reading 20 pages at a time across multiple sessions.
Pages created: Adrian Vermeule, Allan Bloom, Carl Schmitt, Charles Kesler, Christopher Caldwell, Christopher DeMuth, Christopher Rufo, Costin Alamariu, Curtis Yarvin, Darren Beattie, Gladden Pappin, Glenn Ellmers, Harry V. Jaffa, JD Vance, John Eastman, Josh Hammer, Josh Hawley, Julius Krein, Kevin Roberts, Larry P. Arnn, Leo Strauss, Michael Anton, Nathan Pinkoski, Oren Cass, Patrick Deneen, Peter Thiel, R.R. Reno, Richard Spencer, Robert P. George, Ron DeSantis, Sohrab Ahmari, Stephen Miller, Steve Bannon, Tucker Carlson, Viktor Orbán, Yoram Hazony — Fusionism, Hard Right, National Conservatism, Paleoconservatism, Postliberalism, The Claremonters — Catholic Integralism, Common Good Constitutionalism, Decisionism, Declarationism, Esotericism, Ideas First, Longmarcherism, Manosphere, Populism, West Coast Straussianism — 1776 Commission Report, Furious Minds, Integration from Within, On Campus Trump Fans Safe Spaces, Regime Change, The Fight is Now, The Flight 93 Election, Tyranny Inc., Why Liberalism Failed — 2016 Election, Charlottesville 2017, January 6 2021 — American Affairs, Claremont Institute, Compact, First Things, Heritage Foundation, Hillsdale College, Intercollegiate Studies Institute, Journal of American Greatness, Postliberal Order
Pages updated: index.md (fully populated)

## [2026-04-26] ingest | Furious Minds pp. 301–end (Chapters 11–13 complete; full book ingested)
Completed ingest of *Furious Minds* through Chapter 13 (Conclusion: Ecce Furor) and end of book. Material covers: IM-1776/NETTR debate; exposed figures (Pedro Gonzalez, Nate Hochman, Richard Hanania/Hoste); Chapter 12 on Christian nationalism (CFE, NAR/Independent Charismatics, Stephen Wolfe); Chapter 13 conclusion (AEI Mansfield fête July 2022, NatCon 4 July 2024, Trump assassination attempt July 13, Vance VP pick July 15, Biden withdrawal July 21, Deneen's Feb 2025 New College lecture, Field's liberal prescription, Oresteia framing).
Pages created: Christian Nationalism (movement), Harvey Mansfield (thinker), Mike Johnson (thinker)
Pages updated: National Conservatism (NatCon 4 section), Christian Nationalism (Wolfe biography, Christian Reconstructionism, GAE, gynocracy, Fort Lauderdale panel), JD Vance (VP pick, childless cat ladies, Springfield OH), Furious Minds (Chapter 13 full summary), index.md (new pages), IM-1776 (SACR/NETTR already covered in previous session)

## [2026-04-26] ingest | Four new Clippings + one PDF (Tait, Wood, Zerofsky, Kersch)
Sources: (1) "Conservatives or Counterrevolutionaries?" by Joshua Tait (Substack, Aug 2024); (2) "How Bronze Age Pervert Charmed the Far Right" by Graeme Wood (*The Atlantic*, Aug 2023); (3) "How the Claremont Institute Became a Nerve Center of the American Right" by Elisabeth Zerofsky (*NYT Magazine*, Aug 2022); (4) *Beyond Originalism: Conservative Declarationism and Constitutional Redemption* by Ken I. Kersch (*Maryland Law Review*, 2011). Note: Clippings/Untitled.md is an empty clipping (just a URL, same Maryland Law Review article as the PDF); Clippings/llm-wiki.md is the Karpathy meta-document, not a content source — both skipped.
Pages created: Russell Kirk (thinker), M.E. Bradford (thinker), Thomas Klingenstein (thinker), Ryan Williams (thinker), Counterrevolution (concept), Conservatives or Counterrevolutionaries? (text), How Bronze Age Pervert Charmed the Far Right (text), How the Claremont Institute Became a Nerve Center (text), Beyond Originalism (text)
Pages updated: Costin Alamariu (biographical detail from Wood: Newton South HS, MIT, Yale advisors Smith and Garsten, Jewish identity, Emory failure, Brazil/Japan/Spain/Iceland, Wood's personal acquaintance), Harry V. Jaffa (Bradford-Jaffa debate, Reagan NEH nomination, Declarationist Triptych, Philip Jaffa's critique), Claremont Institute (Ryan Williams appointment, Klingenstein profile, Arthur Milikh/Center for American Way of Life, budget ~$9M, donors DeVos/Bradley, fellowship alumni, Clarence Thomas connection, post-Jan 6 split), Declarationism (Kersch's genealogy: Bradford vs. Jaffa, two ideological functions, Declarationist Triptych, Robert P. George/Witherspoon Institute), Paleoconservatism (Sam Francis "Beautiful Losers," M.E. Bradford added, Tait's conservative-to-counterrevolutionary framing), index.md (all new pages)

## [2026-04-26] lint | Full wiki health check
Systematic lint pass across all 91 pages. Findings and fixes:
**Stubs found:** Manosphere (stub tag removed — page is substantive), Joshua Tait (stub retained — genuinely short)
**Orphan pages (0 inbound wikilinks):** On Campus Trump Fans Safe Spaces (fixed: added link in Furious Minds cross-refs); Populism (flagged — not fixed; many prose mentions but no [[Populism]] wikilinks in other pages)
**Broken wikilinks fixed:** [[Kevin D. Roberts]] → [[Kevin Roberts]] (Heritage Foundation.md, National Conservatism.md × 2); [[The Hard Right]] → [[Hard Right]] (Populism.md); [[Patrick Buchanan]] → [[Pat Buchanan]] (2016 Election.md)
**New stub pages created:** Sam Francis (thinker), Paul Gottfried (thinker), Pat Buchanan (thinker), MAGA New Right (concept), The Cathedral (concept), Project 2025 (institution)
**Remaining broken links (no page, flagged for future expansion):** [[Paul Gottfried]] × 6, [[Claremont Review of Books]] × 3, [[Edmund Burke Foundation]] × 3, [[Great Replacement Theory]] × 2, [[Witherspoon Institute]] × 2, [[2020 Election]], [[American Greatness]], [[Bostock v. Clayton County]], [[Clarence Thomas]], [[David Brog]], [[Jared Taylor]], [[Jim DeMint]], [[Matthew Spalding]], [[Rod Dreher]], [[The Virtue of Nationalism]]
**Key unlinked mentions flagged:** Sam Francis (80+ prose mentions, stub created; no wikilinks in existing text — would require mass edit); Project 2025 (9 files, no wikilinks)
**Contradictions flagged (not resolved — structural tensions):** (1) Lincoln interpretation: Declarationist reverence vs. Bradford/neo-Confederate strain coexisting in Claremont ecosystem; (2) Vermeule pre/post-2016 reversal; (3) Deneen Benedict Option → Vermeulean state capture; (4) Populism claims vs. elitist practice
Pages created: Sam Francis, Paul Gottfried, Pat Buchanan, MAGA New Right, The Cathedral, Project 2025
Pages updated: Heritage Foundation, National Conservatism, Populism, 2016 Election, Manosphere (stub tag removed), Furious Minds (On Campus link added), index.md

## [2026-04-26] lint | Populism orphan fix
Added [[Populism]] wikilinks to 5 pages where the concept was discussed without linking: National Conservatism ("economic populists"), Steve Bannon ("populist electoral strategy"), Kevin Roberts ("right-wing populism"), Yoram Hazony ("economic populism"), Regime Change ("hard populist dualities"). Populism.md is no longer orphaned.
Pages updated: National Conservatism, Steve Bannon, Kevin Roberts, Yoram Hazony, Regime Change

## [2026-04-26] synthesis | Overview.md master synthesis written
Wrote the Overview.md master synthesis page tracing the full historical arc from Kirk's Burkean conservatism through the Bradford-Jaffa constitutional civil war to the MAGA synthesis. Integrates the Tait (counterrevolution), Kersch (Declarationism genealogy), and Field (Furious Minds) analytical frames into a seven-section narrative. Key thesis: the MAGA New Right inherited Jaffa's constitutional language while pursuing Bradford's political goals — a specific, traceable incoherence.
Pages updated: Overview.md
