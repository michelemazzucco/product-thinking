# Research: foundation for an idea-validation skill

Source list: [jsumnersmith/product-management](https://github.com/jsumnersmith/product-management). There is one note for each linked resource. All notes use [`_TEMPLATE.md`](_TEMPLATE.md). [`SYNTHESIS.md`](SYNTHESIS.md) merges the notes into the structure for the skill.

**Source types:** `transcript` = the full episode transcript was read. `article` = the full text was read. `secondary` = the original was not available, so author articles, excerpts or summaries were used. Each note has a "Notes on source quality" section with the details.

| # | Source | Code | Note | Type | Status |
|---|---|---|---|---|---|
| 0 | Elad Gil — Product management overview (High Growth Handbook ch. 7) | GIL | [00-elad-gil-pm-overview.md](00-elad-gil-pm-overview.md) | article | Done. 5 chapter pages. The hiring pages were not used. |
| 1 | Marty Cagan — *Inspired* | CAGAN | [books/inspired.md](books/inspired.md) | secondary | Done. SVPG articles: four risks, opportunity assessment, discovery. |
| 2 | Bob Moesta — *Demand-Side Sales 101* | DSS | [books/demand-side-sales.md](books/demand-side-sales.md) | secondary | Done. Re-Wired book summary, JTBD guide, JTBD Radio transcript. |
| 3 | Christensen et al. — *Competing Against Luck* | CHRISTENSEN | [books/competing-against-luck.md](books/competing-against-luck.md) | secondary | Done. Chapter 2 excerpt and HBSWK. The HBR article has a paywall. The HarperCollins page was empty. |
| 4 | Eric Ries — *The Lean Startup* | RIES | [books/lean-startup.md](books/lean-startup.md) | secondary | Done. Ries's blog posts. The MVP types and innovation accounting come only from summaries. |
| 5 | Lenny's Podcast — Karri Saarinen (Linear) | KARRI | [lennys/kari.md](lennys/kari.md) | transcript | Done. Manual captions. |
| 6 | Lenny's Podcast — Shreyas Doshi | SHREYAS | [lennys/shreyas-doshi.md](lennys/shreyas-doshi.md) | transcript | Done. Auto-captions, so the quotes have no punctuation. |
| 7 | Lenny's Podcast — Bob Moesta (JTBD) | MOESTA | [lennys/bob-moesta.md](lennys/bob-moesta.md) | transcript | Done. Manual captions. |
| 8 | Lenny's Podcast — Jeff Weinstein (Stripe) | WEINSTEIN | [lennys/jeff-weinstein.md](lennys/jeff-weinstein.md) | transcript | Done. Manual captions. |
| 9 | Lenny's Podcast — Hamilton Helmer (7 Powers) | HELMER | [lennys/hamilton-helmer.md](lennys/hamilton-helmer.md) | transcript | Done. The episode does not define all 7 powers. |
| 10 | Lenny's Podcast — Ian McAllister (working backwards) | MCALLISTER | [lennys/ian-mcallister.md](lennys/ian-mcallister.md) | transcript | Done. Auto-captions. About half of the episode is career advice. |
| 11 | Invest Like the Best — Patrick & John Collison | COLLISON | [colossus/collison.md](colossus/collison.md) | transcript | **Partial.** YouTube auto-captions for 5 of the 7 clips. Clips #2 (global commerce) and #7 (personal questions) were blocked by HTTP 429. |
| 12 | Invest Like the Best — Andy Rachleff | RACHLEFF | [colossus/rachleff.md](colossus/rachleff.md) | transcript | Done. Official transcript (Wayback Machine copy). |
| 13 | Invest Like the Best — Daniel Ek | EK | [colossus/ek.md](colossus/ek.md) | transcript | Done. Official transcript (Wayback Machine copy). |
| 14 | Invest Like the Best — Systrom & Krieger (Instagram) | KRIEGER | [colossus/krieger.md](colossus/krieger.md) | transcript | Done. Official transcript (Wayback Machine copy). It is a joint interview, so the quotes name the speaker. |
| 15 | Invest Like the Best — Bill Gurley | GURLEY | [colossus/gurley.md](colossus/gurley.md) | transcript | Done. Official transcript (Wayback Machine copy). |
| 16 | 11 Laws of Showrunning — Javier Grillo-Marxuach | SHOWRUN | [articles/showrunning.md](articles/showrunning.md) | article | Done. Full PDF. The product mapping is our interpretation. |
| 17 | Products Are Functions — Ryan Singer | SINGER | [articles/products-are-functions.md](articles/products-are-functions.md) | article | Done. The URL now goes to ryansinger.co. |
| 18 | How Superhuman built a PMF engine — Rahul Vohra | VOHRA | [articles/superhuman-pmf.md](articles/superhuman-pmf.md) | article | Done. |
| 19 | Schumpeter on Strategy — Jerry Neumann | NEUMANN | [articles/schumpeter-strategy.md](articles/schumpeter-strategy.md) | article | Done. |

## Verification done
- All quotes in the 11 transcript notes were checked by a script against the clean transcripts. In the Collison note, some caption errors were fixed and filler words were removed. The note says this.
- The book and article quotes come only from text that the agents fetched. They were not checked again by script.

## Open gaps
- Collison clips #2 and #7. To get them, run `yt-dlp` with `--cookies-from-browser`, or try again later. The video IDs are `H_kOobyDT1U` and `PDMBQZScMBo`.
- None of the 4 books was read. If you have the books, compare the "secondary" notes with them.
