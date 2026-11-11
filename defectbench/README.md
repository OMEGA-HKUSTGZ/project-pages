# DefectBench — OMEGA Lab project page

Project page for **Can Large Multimodal Models Inspect Buildings? A Hierarchical Benchmark for
Structural Pathology Reasoning** (DefectBench), in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2603.20148>
- Code: <https://github.com/Whitneyyyyy/DefectBench>
- Page: <https://omega-hkustgz.github.io/projects/defectbench/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/` in this folder; there is no build step. How to check
and preview it, and the rules for agents, are in the repository's [`README.md`](../README.md)
and [`AGENTS.md`](../AGENTS.md).

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2603.20148v1 (20 Mar 2026). The text paraphrases the abstract and Sections 1, 3 and 4, with the prompts from the appendix (Table 6); it adds no claims. The paper prints the affiliations as author blocks; the superscript numbers group them in the same order. |
| `overview.webp`, `generative-instability.webp`, `segmentation-examples.webp`, `annotation-platform.webp`, `detection-examples.webp` | Figs. 1–5 of the paper (Figs. 4 and 5 are in the appendix), converted from the JPG files in the arXiv source at up to 2400 px wide (`magick -resize`, then `cwebp -q 90`). `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| Defect statistics, Level 1–3 tables, headline numbers | Tables 1–4 of the paper, copied from the LaTeX source. The Level 1 table shows the Q1 columns and the average counting error; the per-class counting columns are left to the paper. Bold marks the best value in each group. |
| What the code repository holds | <https://github.com/Whitneyyyyy/DefectBench> at commit `81a0d48` (10 Apr 2026): evaluation scripts, annotation toolkit, preprocessing scripts, a 50-image data sample. |
| Evidence labels | None: the page has no demos section and no video. The photographs are dataset images with annotations or model outputs drawn on them. |

Not on the page because no public material exists: the full 1,488-image dataset (the repository
holds a 50-image sample), a demo video of the benchmark, and a published venue (the paper is an
arXiv preprint). The repository's screen recording of the annotation tool is not embedded. The
per-class counting errors (Table 2), the source-dataset statistics (Table 5) and the prompt texts
(Table 6) are left to the paper.
