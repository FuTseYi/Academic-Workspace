# Academic Workspace · Maintenance

## Principle

One document, one canonical path. Link across course, meeting and research indexes rather than duplicating substantive content.

## Structure

- `index.html` — Docsify HTML shell and visual design
- `README.md` — homepage
- `_sidebar.md` — main navigation
- `courses/` — 8 course metadata pages; assignment subfolders as needed
- `meetings/` — dated meetings and a reusable template
- `research/` — EPP catalog and future research notes
- `resources/` — cross-course templates and reference links

## Editing protocol

1. Review the source and preserve its terminology and intent.
2. Save a Markdown file to the relevant section, using `YYYY-MM-DD-topic.md` for dated notes.
3. Add a link to the nearest index, then update `_sidebar.md` for frequently accessed documents.
4. Verify relative routes and commit with a descriptive message.
5. Do not publish third-party private proposals, personal contact details, student identities or unpublished work without permission.

## Sources and accuracy

- Course entries were extracted from the 8-row Notion course database on 2026-10-15.
- The UCMP meeting analysis and template originated in the connected Notion workspace.
- EPP catalog is a 2026-10-15 screenshot-based snapshot; named project owners and member counts are intentionally omitted from the public website copy.
- The original 2-page UCMP Assignment 1 PDF is more authoritative than its automatically extracted text, particularly for matrix layouts. Part 2 is not included.

## Deploy

Docsify requires no build. For GitHub Pages, select **Settings → Pages → Deploy from a branch → main / (root)**.

GitHub Pages privacy is distinct from repository privacy; changing an existing public repository to Private does not guarantee that a deployed site is access-restricted.
