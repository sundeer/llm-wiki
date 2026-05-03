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

## [2026-04-26] lint | Second full health check
Inbox: empty. Orphans: none. Stubs resolved and broken links fixed from the previous lint's flagged list.
**Broken links fixed:** [[Chris DeMuth]] → [[Christopher DeMuth]] (National Conservatism.md); [[Harvey C. Mansfield]] → [[Harvey Mansfield]] (Harry V. Jaffa.md, Leo Strauss.md); [[Intercollegiate Studies Institute|Edmund Burke Foundation]] → [[Edmund Burke Foundation]] (Christian Nationalism.md — these are separate organizations).
**File rename:** "Tyranny Inc.md" → "Tyranny, Inc.md" (filename now matches frontmatter title and all wikilinks).
**De-stubbed (pages were fully developed):** Pat Buchanan, Sam Francis, Paul Gottfried, The Cathedral, Project 2025.
**New pages created:** Edmund Burke Foundation (institution), The Virtue of Nationalism (text), Laura K. Field (thinker), Claremont Review of Books (institution), American Greatness (institution), Rod Dreher (thinker), Schedule F (concept), 2020 Election (event).
**Remaining broken links (low-priority, flagged for future expansion):** [[David Brog]], [[Clarence Thomas]], [[Jared Taylor]], [[Jim DeMint]], [[Matthew Spalding]], [[Witherspoon Institute]], [[Great Replacement Theory]], [[Bostock v. Clayton County]].
Pages created: Edmund Burke Foundation, The Virtue of Nationalism, Laura K. Field, Claremont Review of Books, American Greatness, Rod Dreher, Schedule F, 2020 Election
Pages updated: National Conservatism, Harry V. Jaffa, Leo Strauss, Christian Nationalism, Pat Buchanan, Sam Francis, Paul Gottfried, The Cathedral, Project 2025, index.md

## [2026-04-27] ingest | *Republic* by Plato (Grube/Reeve trans., Hackett 1992) — full text (313 pages, all 10 books)
Source: Raw/Republic -- Plato.pdf. Full systematic read across 16 sessions (pages 1–313). The Republic is the primary ancient source for the New Right's anti-democratic political theory, transmitted primarily through Strauss's esotericism, Bloom's cultural critique, and BAP's inverted Platonic reading.
Key passages annotated for New Right relevance: Noble Lie/Myth of Metals (414b-415d); Cave Allegory (514a-520a); Ship of State (488a-489d); Knowledge vs. Opinion / anti-democratic epistemology (476a-480a); Democratic Degeneration → Tyranny (Books VIII-IX, esp. "extreme freedom leads to extreme slavery," 564a); Philosopher-King passage (473c-d); Damon thesis / culture precedes politics (424c); Two cities at war (422e); "Divine reason imposed from without" / common good (590d); City in heaven / impossibility of ideal city (592b); Beast within / tyrannical-erotic soul (571b-572b, 573a); Chimera of the soul (588b-591b); Choice of Lives / Myth of Er (617d-621d).
Pages created: Republic (text), Plato (thinker)
Pages updated: Leo Strauss (new section: "Strauss's Reading of Plato's Republic"), Costin Alamariu (new section: "BAP's Platonic Reading: Thymos against Logos"), index.md

## [2026-04-30] lint | Inbox + orphans + missing-page sweep
Inbox empty (no triage required). Tackled outstanding orphans/missing pages and stub backlog.
Pages created: Administrative State (concept), Great Replacement Theory (concept), Clarence Thomas (thinker), David Brog (thinker), Jared Taylor (thinker), Jim DeMint (thinker), Matthew Spalding (thinker), Witherspoon Institute (institution) — 8 stubs spun up from longstanding wikilink targets that previously resolved to nothing
Pages updated: Curtis Yarvin, Russell Kirk, Sam Francis, Counterrevolution, "Conservatives or Counterrevolutionaries?" (wikified plain-text "Joshua Tait" mentions to fix the Joshua Tait orphan); index.md (new entries in Thinkers, Concepts, Institutions)
Flagged for follow-up: stub expansion needed for Joshua Tait, Laura K. Field, Rod Dreher, Schedule F, 2020 Election, American Greatness, Claremont Review of Books, Edmund Burke Foundation, The Virtue of Nationalism — all are real pages with substantive [stub] tags awaiting fuller treatment. Also: `[[Bostock v. Clayton County]]` is a single-link target in Josh Hammer's "Related" section; consider whether to create a court-case stub or unlink (Hammer's body already explains *Bostock* in detail). False-positive orphan: `Wiki/Texts/Tyranny, Inc.md` shows as unlinked due to filename punctuation (basename `Tyranny, Inc` vs link text `Tyranny, Inc.`); Obsidian resolves these; safe to ignore.

## [2026-05-03] lint | Inbox + broken-link sweep
Inbox: empty (only .gitkeep). Orphans: none. All 91 wiki pages reachable.
**Broken links fixed (2 remaining, now 0):**
- `[[James Madison Program]]` — created institution stub (referenced as a substantive node by Witherspoon Institute, Robert P. George, Adrian Vermeule, Nathan Pinkoski).
- `[[Bostock v. Clayton County]]` — unlinked the single occurrence in Josh Hammer's "Cross-References" (no court-case category; Hammer body covers Bostock fully).
**Stub backlog (no change, 17 pages still tagged `[stub]`):** Witherspoon Institute, American Greatness, Edmund Burke Foundation, Claremont Review of Books, Matthew Spalding, David Brog, Joshua Tait, Jim DeMint, Laura K. Field, Rod Dreher, Clarence Thomas, Jared Taylor, The Virtue of Nationalism, Great Replacement Theory, Schedule F, Administrative State, 2020 Election. All are real pages; flagged for expansion when the relevant source is read.
**New ingest backlog flagged (not processed by lint):** 8 untracked clippings sit in `Clippings/` awaiting `/ingest`: "Debunking a Longstanding Myth About William F. Buckley", "Democracy Faces a Reactionary Counter-Mobilization", "I Thought I Understood the American Right. Trump Proved Me Wrong.", "Long before QAnon, Ronald Reagan and the GOP purged John Birch extremists from the party", "The Conservative Consensus: Frank Meyer, Barry Goldwater, and the Politics of Fusionism", "The New Lost Cause", "'America Is a Republic, Not a Democracy' Is a Dangerous—And Wrong—Argument", "'I Don't Want to Violently Overthrow the Government. I Want Something Far More Revolutionary.'"
**Mentioned-but-no-page candidates (load-bearing):** Stephen Wolfe (3 pages, central to Christian Nationalism); New Apostolic Reformation / Independent Charismatics (11 mentions on Christian Nationalism alone); Christian Reconstructionism (Rushdoony lineage). All flow through Christian Nationalism; recommend page creation on next ingest pass touching that material.
**Contradictions / structural tensions (carried forward, unchanged):** Lincoln interpretation (Declarationist vs. Bradford strain); Vermeule pre/post-2016; Deneen Benedict Option → state capture; Populism rhetoric vs. elitist practice.
Pages created: James Madison Program (institution stub)
Pages updated: Josh Hammer (Bostock unlinked), index.md (James Madison Program added)

## [2026-05-03] ingest | Eight new clippings (3 thematic clusters)
Processed all eight new untracked clippings in `Clippings/` in three thematic clusters. Wiki page count: 91 → 132. Zero broken wikilinks.

### Cluster A — Buckley / John Birch Society (Dallek vs. Trickey)
Sources: (1) "Debunking a Longstanding Myth About William F. Buckley" by Matthew Dallek (*Politico Magazine*, March 2023; excerpt from *Birchers: How the John Birch Society Radicalized the American Right*, Basic Books 2023); (2) "Long before QAnon, Ronald Reagan and the GOP purged John Birch extremists from the party" by Erick Trickey (*Washington Post* "Retropolis," January 2021).
Direct contradiction: Trickey retells the standard "Buckley purged the Birchers" narrative; Dallek demolishes it (citing political scientists Daniel Schlozman and Sam Rosenfeld). The wiki sides with Dallek — Buckley targeted Welch personally while courting the rank-and-file ("I don't think in my life I have made a single unfavorable reference to any members of the John Birch Society"). The "purge" was performative; the underlying Bircher politics stayed inside the conservative tent. This strengthens the wiki's existing Tait/Counterrevolution thesis: the post-2016 mainstreaming of conspiracism is *resurfacing*, not *return*.
Pages created: Texts: Debunking a Longstanding Myth About William F. Buckley, Long before QAnon Ronald Reagan…; Institutions: John Birch Society; Thinkers: William F. Buckley Jr., Robert Welch, Barry Goldwater (initial stub), Matthew Dallek (stub).
Pages updated: Counterrevolution (new "Buckley/Birch Case Study" section), Russell Kirk (Palm Beach 1962), Josh Hammer (unlinked Bostock per lint), Overview.md (Section II paragraph on Buckley/Birch revisionism).

### Cluster B — Fusionism (Edwards / Heritage 2007)
Source: "The Conservative Consensus: Frank Meyer, Barry Goldwater, and the Politics of Fusionism" by Lee Edwards (Heritage Foundation report, January 2007).
Major findings: Frank Meyer canonized as fusionism's intellectual father; *In Defense of Freedom* (1962); the 1964 *What Is Conservatism?* volume. **Critical datum**: Edwards reveals that Harry Jaffa drafted Goldwater's 1964 "ordered liberty" passage — Jaffa was therefore the constitutional theologian of mainstream fusionist Republican conservatism in 1964, not just an academic Straussian; this contextualizes his entire West Coast Straussian phase. **Bozell datum**: L. Brent Bozell Jr. (Buckley's brother-in-law, ghostwriter of *The Conscience of a Conservative*) wrote a 1962 essay arguing "the purpose of politics… is not the promotion of freedom but the promotion of virtue and the building of 'a Christian civilization'" — direct ancestor of Vermeule/Deneen/Ahmari postliberalism, the position fusionism defeated and that returned post-1991. **Hayek datum**: "Why I Am Not a Conservative" (1960) accurately described what conservatism would become — coercion for moral ends, "strident nationalism" as "bridge to collectivism." **Heritage 2007→2025 self-reversal**: the same institution that in 2007 prescribed "renewed fusionism" published Project 2025 in 2023 — structurally incompatible programs in the same building.
Pages created: Texts: The Conservative Consensus, The Conscience of a Conservative; Thinkers: Frank Meyer, Ronald Reagan, L. Brent Bozell Jr.
Pages updated: Fusionism (substantial rewrite — added Meyer/Bozell/Hayek/anti-communist-cement framing and Heritage self-reversal); Barry Goldwater (de-stubbed, full expansion: *Conscience*, 1964 campaign, Bircher episode, later career); Harry V. Jaffa ("ordered liberty" drafter datum); Russell Kirk (Meyer-Kirk feud); Heritage Foundation (2007→2025 trajectory section); Overview.md (Section VI Heritage paragraph).

### Cluster C — Synthesis-level pieces (Thomas, Ward/Deneen, Graham, Perlstein, Zimmer)
Sources: (1) "'America Is a Republic, Not a Democracy' Is a Dangerous — And Wrong — Argument" by George Thomas (*Atlantic*, November 2020); (2) "'I Don't Want to Violently Overthrow the Government. I Want Something Far More Revolutionary.'" by Ian Ward (*Politico Magazine*, June 2023, profile of Patrick Deneen); (3) "The New Lost Cause" by David A. Graham (*Atlantic*, October 2021); (4) "I Thought I Understood the American Right. Trump Proved Me Wrong." by Rick Perlstein (*NYT Magazine*, April 2017); (5) "Democracy Faces a Reactionary Counter-Mobilization" by Thomas Zimmer (Substack, November 2022).
Major findings: **Thomas** is the cleanest single rebuttal of the Claremont/MAGA "republic not democracy" formula (Madison/Hamilton/Lincoln evidence; "minority rule, as a permanent arrangement, is wholly inadmissible"). **Ward/Deneen** is biographical — Rutgers/Carey McWilliams (left-communitarian mentor) → Princeton tenure denial 2004 → Catholic turn → Notre Dame 2012 → Orbán meeting 2019; introduces "common-good conservatism" (distinct from NatCon), "aristopopulism," "Party of Order vs. Party of Progress" (uncredited Saint-Simonian/Comtean borrowing); Field's frame: "illiberal constitutionalism." **Graham** documents the New Lost Cause as conscious heir of the Confederate Lost Cause: martyr cult (Babbitt), J6 flag veneration, "high water mark" mythologization. **Perlstein** is a self-reckoning by the historian whose *Before the Storm* helped build the "respectable rise" consensus — concedes the framework was systematically too narrow (1920s Klan, Christian Front, Trump père NYC racism, herrenvolk republicanism); concordant with Dallek and Tait. **Zimmer** offers vocabulary upgrade: "reactionary counter-mobilization" rather than "backlash," restoring agency.
Pages created: Texts: America Is a Republic Not a Democracy, I Don't Want to Violently Overthrow the Government, The New Lost Cause, I Thought I Understood the American Right, Democracy Faces a Reactionary Counter-Mobilization; Thinkers: Wilson Carey McWilliams (stub), Rick Perlstein (stub).
Pages updated: Patrick Deneen (substantial — added biographical formation section, common-good-vs-NatCon distinction, Party of Order/Progress, transitional policy list, "for me it wouldn't be" J6 disavowal); Regime Change (Party of Order/Progress, transitional policies, illiberal constitutionalism); Declarationism ("Republic Not a Democracy" deployment section); January 6 2021 (New Lost Cause section); Counterrevolution (Cluster C cross-references).

### Aggregate touch counts
Pages created (this ingest): 17 — 11 Texts, 8 Thinkers, 1 Institution. (Texts: 7; Institutions: 1; Thinkers: 8 = Buckley Jr., Welch, Goldwater, Dallek, Meyer, Reagan, Bozell, McWilliams, Perlstein.)
Pages updated: 14 — Counterrevolution, Russell Kirk (×2), Josh Hammer, Harry V. Jaffa, Heritage Foundation, Fusionism, Patrick Deneen, Regime Change, Declarationism, January 6 2021, index.md, Overview.md.

### Overview revisions
Two paragraphs added: Section II (Buckley/Birch revisionism strengthens the continuity reading); Section VI (Heritage 2007→2025 self-reversal as institutional indicator of the systemic shift).

### Stubs flagged for future expansion
New stubs: Matthew Dallek, Rick Perlstein, Wilson Carey McWilliams. Plus carryover from prior lints. Total stub count: 19.

### Synthesis assessment
The Cluster A and Cluster F findings (Dallek + Perlstein) substantially **strengthen** the wiki's existing Counterrevolution thesis without revising it; they were absorbed into existing pages with one Overview paragraph each. The Cluster B finding (Heritage 2007→2025) is the most synthesis-relevant addition — it gives the Overview a clean institutional anchor for the framework-shift claim. The Cluster D (Deneen biographical) and Cluster E (New Lost Cause) findings expanded individual pages but didn't require Overview revision. No source surfaced a contradiction with the existing synthesis.
