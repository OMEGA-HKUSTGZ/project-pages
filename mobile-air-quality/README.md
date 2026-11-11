# Mobile Air-Quality Mapping — OMEGA Lab project page

Project page for **High-resolution urban air pollution and thermal comfort mapping: an
application of drive mobile sensing platform for smart city services**, in the OMEGA Lab style.

- Paper: <https://arxiv.org/abs/2412.17831>
- Page: <https://omega-hkustgz.github.io/projects/mobile-air-quality/> (live once the lab site lists it)

## Working on the page

The page is `index.html` plus `assets/` in this folder; there is no build step. How to check
and preview it, and the rules for agents, are in the repository's [`README.md`](../README.md)
and [`AGENTS.md`](../AGENTS.md).

## Sources

Everything on the page comes from public material. Keep this list current.

| On the page | Source |
| --- | --- |
| Title, authors, affiliations, text | arXiv 2412.17831v3 (3 Jun 2025; first submitted 13 Dec 2024). The text paraphrases the abstract and Sections 2–4; it adds no claims. The title is written as in the arXiv listing. Authors, superscripts and affiliations are as printed on the title page, which lists affiliations a, b and c only. |
| `study-area.webp`, `station-comparison.webp`, `exposure-disparity.webp`, `weekly-pattern.webp`, `road-type-pattern.webp`, `hourly-maps.webp`, `exposure-levels.webp` | Figs. 1–7 of the paper. The authors uploaded a PDF only, so these are the images embedded in it (`pdfimages -j`, about 1500 px wide, not enlarged), converted with `cwebp -q 90`. `social.jpg` is Fig. 1 on a 1200 × 630 canvas for link previews. |
| `instruments.webp` | Fig. S1 of the paper, cropped to its instrument panels (sensor assembly, sensor testing and the two photographs below them). |
| Instrument table, exposure-level table | Table 1 and Table S1 of the paper, copied from the PDF. |
| By-pollutant table and headline numbers | Numbers stated in the text of Sections 2.1, 2.3, 3.1 and 3.3 of the paper, copied as written. The paper has no single table with them; the page collects them by pollutant. |

Not on the page because no public material exists: code, the measurement dataset and any demo
video. The supplementary figures on mean against median (Fig. S2), the per-station statistical
metrics (Fig. S3) and the temperature and humidity curves (Fig. S4) are left to the paper.
