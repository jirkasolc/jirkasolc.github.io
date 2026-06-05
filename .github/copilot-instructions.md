# Copilot instructions

This repository is a single-page static website. The entire site is built from `index.html`; HTML and CSS are colocated in one file.

- Use `index.html` as the primary source of truth. All sections, layout, and styling are defined there.
- There is no JavaScript, Node.js, or build pipeline. Do not introduce a toolchain unless explicitly requested.
- The site is intended for GitHub Pages. Local preview is done by opening `index.html` in a browser.
- Preserve the existing structure:
  - `.container` wraps page sections
  - `.divider` separates major page blocks
  - `.hero`, `.cards`, `.timeline`, `.learning-grid`, `.cert-groups`, `.tags`, and `footer` are the main content patterns
- Style changes should use the existing CSS variables in `:root` when possible (`--bg`, `--surface`, `--accent`, etc.).
- Keep layout patterns consistent:
  - grid-based cards and timelines
  - responsive breakpoints using `@media (max-width: 520px)`
- Content updates should remain semantic and simple: headings, paragraphs, links, and small inline emoji icons.
- Do not split the file into multiple assets without approval. The current site is intentionally minimal.
- `README.md` is a placeholder and should not be treated as the canonical website content.

If a requested change needs a larger restructuring, ask for clarification before adding new files or build steps.