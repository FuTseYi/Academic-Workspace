# Academic Workspace · Maintenance Guide

This repository is a **Markdown-first static documentation site** powered by Docsify 4.

## Content structure

```text
/
├── index.html          # Docsify shell and appearance
├── README.md           # Website home
├── _sidebar.md         # Global navigation
├── .nojekyll           # Keep underscore-prefixed files on GitHub Pages
├── courses/
│   ├── README.md
│   └── UCMP-6050.md
├── meetings/
│   └── README.md
├── research/
│   └── README.md
└── resources/
    └── README.md
```

## How to add a document

1. Decide where the document belongs: `courses/`, `meetings/`, `research/`, or `resources/`.
2. Use a descriptive slug: `YYYY-MM-DD-short-topic.md` for dated documents; use `README.md` for a category landing page.
3. Create a complete Markdown document with a clear title, date (when useful), source links and an action section (when applicable).
4. Link it from its section index; add it to `_sidebar.md` only if it should be in the global navigation.
5. Commit with a scoped message, e.g. `docs(ucmp): add meeting notes`.

Prefer links over duplicated documents. Store screenshots or supporting images in a nearby `assets/` folder when needed. Keep file paths stable so existing links do not break.

## Website publishing

GitHub repository: https://github.com/FuTseYi/Academic-Workspace

For GitHub Pages, open **Settings → Pages**; choose **Deploy from a branch**; branch **main**, folder **/(root)**; save. The expected URL for a project site is https://futseyi.github.io/Academic-Workspace/ after Pages is enabled and deployment succeeds.

No build command or GitHub Actions workflow is required.

Local preview (if desired):

```bash
python -m http.server 3000
```

Then open `http://localhost:3000/` from the repository root.

## Privacy safeguards

- **Current repository visibility: public.** Do not commit non-public Notion exports, classmates' contact details, instructor feedback, personal AS considerations, draft applications, or private proposal details while the repository remains public.
- GitHub Pages **does not become access-restricted simply because the repository is switched to private**. Confirm the deployment/access policy separately before posting restricted content.
- Making a public repository private later cannot retract already copied or indexed material.
- Treat public material as intentional publication; verify licensing and permissions for third-party course material.

## Future update workflow

Discuss → draft/verify → choose folder → commit Markdown and update index/sidebar → GitHub Pages automatically republishes after the publishing source is configured.
