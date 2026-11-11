# Battery-Efficient UAV Delivery Routing — OMEGA Lab project page

Project page for **Robust Energy-Aware Routing for Air-Ground Cooperative Multi-UAV Delivery in
Wind-Uncertain Environments** (BER), in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2604.13441>
- Page: <https://omega-hkustgz.github.io/projects/battery-efficient-uav-routing/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/` in this folder; there is no build step. How to check
and preview it, and the rules for agents, are in the repository's [`README.md`](../README.md)
and [`AGENTS.md`](../AGENTS.md).

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2604.13441v1 (15 Apr 2026, cs.RO). The text paraphrases the abstract and Sections I, III, IV, V, VI and VII; it adds no claims. The paper carries the line "This work has been submitted to the IEEE for possible publication" and the arXiv record states no venue or publisher DOI, so no venue is cited and the citation is `@misc`. |
| `teaser.webp`, `wind-model.webp`, `framework.webp`, `maddpg-network.webp`, `energy-per-distance.webp`, `sensitivity.webp` | Figs. 1, 2, 3, 4, 5 and 6 of the paper, rendered from the arXiv source PDFs at 2400 px wide (`pdftoppm -cropbox -scale-to 2400`, then `cwebp -q 90`), unaltered. `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| Mission-outcome table, headline numbers | Table I of the paper, copied from the LaTeX source and laid out with one row per method instead of one column group per method. "Approximately 3–8%" and "over 67%" are the paper's own words in Section VI-B. The ablation numbers in the text (92.4% and 74.6%) are from Table II and Section VI-C. |
| Evidence labels | Every experiment in the paper is a simulation: Erdős–Rényi graphs abstracted from Unreal Engine 4 scenes, with replayed wind logs the paper calls "quasi-real". Fig. 1(b) is the simulated delivery environment and Fig. 2(a) a view of the simulator (both Simulation); the other panels and Figs. 3–6 are diagrams and charts. The paper reports no flights and no hardware. |
| Later preprint (one sentence in the scope paragraph) | arXiv 2608.11641 by the same authors, linked without claiming a version relationship; neither paper states one. |

Not on the page because no public material exists: a code repository for this paper (so there is
no Code button; the authors' public repository `The-EWR-UAV-Routing` belongs to the later
preprint), a demo video, flight-test footage (the paper reports simulation only), the experiment
data behind the tables, and a published-venue record. The ablation table (Table II) is left to the
paper.
