# Intention-Driven Lane Change — OMEGA Lab project page

Project page for **An Intention-Driven Lane Change Framework Considering Heterogeneous Dynamic
Cooperation in Mixed-Traffic Environments**, in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2509.22550>
- Journal version: <https://doi.org/10.1109/TITS.2026.3690192> (IEEE Transactions on Intelligent Transportation Systems)
- Page: <https://omega-hkustgz.github.io/projects/intention-lane-change/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/` in this folder; there is no build step. How to check
and preview it, and the rules for agents, are in the repository's [`README.md`](../README.md)
and [`AGENTS.md`](../AGENTS.md).

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2509.22550v4 (17 Mar 2026), published in IEEE Transactions on Intelligent Transportation Systems, 2026, DOI 10.1109/TITS.2026.3690192. The title is as printed on the paper and at IEEE. The text paraphrases the abstract and Sections III–VI; it adds no claims. The affiliation numbers 1 and 2 stand for the paper's two unnumbered affiliation footnotes. |
| `framework.webp`, `style-clusters.webp`, `cooperation-composition.webp`, `cooperation-profile.webp`, `case-irl-prediction.webp`, `case-idm-prediction.webp` | Figs. 1, 2, 4(a), 4(b), 5(a) and 5(b) of the paper, from the PNG files in the arXiv source: flattened on white, resized to at most 2400 px wide with `magick`, then `cwebp -q 90`. `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| NGSIM and motion-planning tables, headline numbers, highD, inference-time and ablation numbers | Tables III and VII of the paper as tables; numbers in the text from Tables IV, V and VI and Sections V-D and V-E; all copied from the LaTeX source. |
| Evidence labels | Figs. 5(a) and 5(b) show one simulated lane change: the ego vehicle is driven by the planner, the surrounding vehicles follow recorded NGSIM I-80 trajectories (Simulation). The decision results (Tables III–VI) are computed on recorded trajectory datasets (NGSIM I-80, highD); the paper has no real-vehicle experiment. |

Not on the page because no public material exists: a code repository (so there is no Code
button), demo video, and trained weights. Fig. 3 (training curves and confusion matrix), Fig. 6
(control inputs) and Tables I, II, IV–VI and VIII are left to the paper.
