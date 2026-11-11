# PLAN-S — OMEGA Lab project page

Project page for **PLAN-S: Bridging Planning with Latent Style Dynamics for Autonomous Driving
World Models**, in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2606.06014>
- Page: <https://omega-hkustgz.github.io/projects/plan-s/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/` in this folder; there is no build step. How to check
and preview it, and the rules for agents, are in the repository's [`README.md`](../README.md)
and [`AGENTS.md`](../AGENTS.md).

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliation, text | arXiv 2606.06014v1 (4 Jun 2026). The text paraphrases the abstract and Sections I, III, IV and V; it adds no claims. |
| `style-cost-maps.webp`, `framework.webp`, `difficulty.webp`, `qualitative.webp` | Figs. 4, 1, 2 and 3 of the paper, converted from the PNG files in the arXiv source at their original size (`cwebp -q 90`). `social.jpg` is Fig. 4 on a 1200 × 630 canvas for link previews. |
| nuScenes and NAVSIM tables, headline numbers | Tables I and V of the paper, copied from the LaTeX source. In the nuScenes table the page highlights the best value in each column, including ties; the paper bolds the whole PLAN-S row. The NAVSIM table keeps the paper's highlighting. Numbers in the text are from Tables I, II–IV and VI–X. |
| Evidence labels | None. Every figure is a paper figure from evaluation on recorded benchmark data (nuScenes, NAVSIM); the page has no demos section and shows no robot or vehicle run. |

Not on the page because no public material exists: a code repository (so there is no Code
button), demo video, and released weights. The ablation tables (Tables II, III, VI and VII) and
the hard-subset and oracle diagnostics (Tables IX and X) are left to the paper.
