# project-pages

Lab standard: <https://github.com/OMEGA-HKUSTGZ/.github-private/blob/main/STANDARD.md>

## 这是什么

The lab's project pages, one folder per project. omega-lab-site publishes each folder it
lists in its `project-pages.json` at `https://omega-hkustgz.github.io/projects/<folder>/`.
Pages start from the lab's project-page template:
<https://github.com/OMEGA-HKUSTGZ/.github/tree/main/templates/project-page>.

## 写在哪里

- One page: `<slug>/index.html`, media in `<slug>/assets/media/`. The folder name is the slug.
  No build step.
- Styles and scripts only that page needs: `<slug>/assets/css/page.css` and a new file in
  `<slug>/assets/js/`.
- Where each figure, number and clip comes from: `<slug>/README.md`.
- Do not edit the shared files here: `tools/`, and in every page
  `assets/css/omega-page.css`, `assets/js/omega-page.js`, `assets/fonts/`, `assets/brand/`.
  Change them in the template, then refresh with
  `node <.github checkout>/templates/project-page/new-page.mjs . --update`.
- A new page: `node <.github checkout>/templates/project-page/new-page.mjs <slug> --slug <slug> --title "<Title>"`,
  on a branch, as a pull request.

## 怎么检查

```sh
node tools/check.mjs
```

CI runs the same command; it checks every page. Look at the pages with `node tools/serve.mjs`
at desktop and phone widths. A pull request gets a preview at
`https://omega-hkustgz.github.io/preview/project-pages-pr-<number>/<slug>/`.

## 坑

- Text, numbers and figures come from the public paper and released material. Copy numbers
  from the paper's source; do not round up, extrapolate or add claims.
- Every clip and photo of a run says what it is: `data-evidence` is `simulation`, `hil`,
  `real-world` or `animation`, with the matching visible tag. Simulated motion driven by real
  onboard hardware is `hil`, not `real-world`. No material, no section.
- Each page is published two levels deep: lab links are `../../`, everything else is a path
  relative to the page's own folder. A page never loads a file from another page's folder.
- Leave `<meta name="robots" content="index, follow">`; previews are made noindex by CI.
- A file over 20 MiB, or over 50 MB of media in one page, goes to a lab media repository.
- A draft stays on its branch until its authors confirm it. A page goes live only when
  omega-lab-site lists it in `project-pages.json`.
