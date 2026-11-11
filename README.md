# OMEGA Lab project pages

One folder per research project. Each folder is a static page in the OMEGA Lab style that
`omega-lab-site` publishes at `https://omega-hkustgz.github.io/projects/<folder>/` once the
page is listed in its `project-pages.json`:

```json
{ "slug": "<folder>", "repository": "OMEGA-HKUSTGZ/project-pages", "path": "<folder>" }
```

## Working on a page

A page is `<folder>/index.html` plus `<folder>/assets/`; there is no build step. Where its
text, numbers and figures come from is in `<folder>/README.md`. Rules for agents are in
[`AGENTS.md`](AGENTS.md).

```sh
node tools/check.mjs     # what CI runs: every page
node tools/serve.mjs     # look at the pages locally
```

## From draft to live

1. A draft is written from the public paper and released code, on a branch, and opened as a
   pull request. The pull request gets a preview at
   `https://omega-hkustgz.github.io/preview/project-pages-pr-<number>/<folder>/`
   (not indexed, marked as a draft, removed when the pull request closes).
2. The authors look at the preview and confirm, or say what to change.
3. The confirmed page is merged to `main`, and `omega-lab-site` lists it. A pull request that
   holds several drafts is merged page by page: `git checkout <draft branch> -- <folder>` on a
   branch from `main`.

Starting a page, the shared files and what the check enforces:
<https://github.com/OMEGA-HKUSTGZ/.github/tree/main/templates/project-page>.

`unit-page`, `lightvln-page` and `commit-while-futures-agree-page` were started before this
repository and are still repositories of their own.
