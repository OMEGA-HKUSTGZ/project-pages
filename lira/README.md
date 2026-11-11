# LIRA — OMEGA Lab project page

Project page for **LIRA: Local Cross-Layer Information Routing for Vision-Language-Action
Decoding**, in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2608.07596>
- Page: <https://omega-hkustgz.github.io/projects/lira/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/` in this folder; there is no build step. How to check
and preview it, and the rules for agents, are in the repository's [`README.md`](../README.md)
and [`AGENTS.md`](../AGENTS.md).

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, author marks, text | arXiv 2608.07596v1 (6 Aug 2026). The text paraphrases the abstract, the method, experiment and real-world sections and the conclusion; it adds no claims. The paper prints no institutional affiliations, so the page lists only its three author marks (equal contribution, project lead, corresponding author). |
| `teaser.webp`, `framework.webp`, `ablations.webp`, `platform.webp` | Figs. 1–4 of the paper, from the arXiv source: Figs. 1 and 2 rendered from the vector PDFs at about 2400 px wide (`pdftoppm`, then `cwebp -q 90`); Figs. 3 and 4 converted from the source PNG/JPG at 2400 px wide (`magick`, then `cwebp -q 90`). `social.jpg` is Fig. 1 on a 1200 × 630 white canvas for link previews. |
| LIBERO-Plus, LIBERO, CALVIN and real-robot tables, headline numbers | Tables 4, 2, 3 and 9 of the paper, copied from the LaTeX source; bold cells follow the paper's own bold. The ablation and resource sentences quote Tables 5–8. |
| Evidence labels | Fig. 1 shows LIBERO-Plus rollout frames, a simulation benchmark: labelled Simulation. Fig. 4 is a photograph of the physical Franka Research 3 platform used for the real-robot evaluation: labelled Real-world, and the caption says it is a photograph of the setup. |
| Code statement | The arXiv comment: code and model checkpoints will be released upon acceptance of the paper. |

Not on the page because no public material exists: a code repository (so there is no Code
button), model checkpoints, demo video and frames or footage of the real-robot trials (the
paper shows only the platform photograph). The related-work comparison (Table 1) and the
ablation and resource tables (Tables 5–8) are left to the paper.
