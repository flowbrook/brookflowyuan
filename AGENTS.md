# AGENTS.md

## Cursor Cloud specific instructions

This repository is a single, zero-dependency static website (`index.html` plus `README.md`). All HTML, CSS, and JavaScript are inline in `index.html`; there is no package manager, build step, backend, database, or automated test suite.

- Serve locally for development/preview with `python3 -m http.server 8000` from the repo root, then open `http://localhost:8000/` (documented in `README.md`). The page can also be opened directly as a `file://`.
- There are no dependencies to install, nothing to build, and no lint or test commands. "Testing" means opening the page in a browser and verifying rendering plus the inline JS interactions (sticky nav anchor links with smooth scroll, mobile nav toggle, `Escape` handling, and `IntersectionObserver` reveal animations that respect `prefers-reduced-motion`).
- No environment variables or secrets are required.
