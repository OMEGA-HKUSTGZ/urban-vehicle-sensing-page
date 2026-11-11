# Vehicle-Based Urban Sensing — OMEGA Lab project page

Project page for **Enhancing Urban Sensing Utility with Sensor-enabled Vehicles and Easily
Accessible Data** (IEEE ITSC 2025), in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2512.07124>
- Published version: <https://doi.org/10.1109/ITSC60802.2025.11423491>
- Page: <https://omega-hkustgz.github.io/projects/urban-vehicle-sensing/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/`; there is no build step. Rules for agents are in
[`AGENTS.md`](AGENTS.md).

```sh
node tools/check.mjs     # what CI runs
node tools/serve.mjs     # look at it locally
```

Every pull request gets a preview link, posted on the pull request. A push to `main` asks the
lab site to republish.

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2512.07124v1 (8 Dec 2025). The text paraphrases the abstract and Sections I, III, IV and V; it adds no claims. The paper marks the corresponding author in a footnote, without a symbol, so the page names him in a line under the affiliations. |
| Venue, pages and DOI in the button and the BibTeX | The lab site's `publications.json` record, verified there against Crossref: 2025 IEEE 28th International Conference on Intelligent Transportation Systems (ITSC), pp. 3218–3223, DOI 10.1109/ITSC60802.2025.11423491. The arXiv abstract page lists no journal reference. |
| `weights-framework.webp`, `estimation-errors.webp`, `error-maps.webp`, `weight-ablation.webp` | Figs. 1–4 of the paper, rendered from the arXiv source PDFs with the long side at 2400 px (`pdftoppm`, then `cwebp -q 90`). `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| Sensing-utility table, headline numbers | Table I of the paper, copied from the LaTeX source; bold marks are the paper's own. "6 of 7" counts the columns of Table I in which Improved OptiFleet is bold. The 200- and 250-vehicle error thresholds, the study area, grid and data description are from Sections IV-A and IV-B. |
| Evidence labels | None needed: the figures are a method diagram, plots and maps computed from recorded data, not footage of a run. |

Not on the page because no public material exists: a code repository (so there is no Code
button), the taxi trajectory and air quality data, and any demo or video (so there is no demos
section). The related journal article in Transportation Research Part C (2026) is a separate
publication and is not described here.
