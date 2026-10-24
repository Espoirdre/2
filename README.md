# Espoirdre — GitHub homepage

Source for <https://espoirdre.github.io/>. A single static page: one HTML file,
no build step, no dependencies (so there is no dependency manifest or lockfile to
include).

## Files

```
index.html   the whole site — markup, CSS and the inline SVG favicon
README.md    this file
```

## How to preview it

**Option 1 — open the file.** Double-click `index.html`, or drag it into any
browser. Everything works offline; nothing is loaded from the network.

**Option 2 — local server** (closer to how GitHub Pages serves it):

```bash
python -m http.server 8000
# then open http://localhost:8000/
```

## How it is published

The repository is named `Espoirdre.github.io`, `index.html` sits at the
repository root, and GitHub Pages deploys the `main` branch from `/` (root).
Any push to `main` republishes the site within a minute or two.

## Page behaviour

- Responsive down to narrow phone widths.
- Follows the reader's light/dark preference via `prefers-color-scheme`.
- Respects `prefers-reduced-motion` (the entrance animation is skipped).
- Contains no analytics, cookies, trackers or third-party requests.

No personal identifiers are published here: no student ID, no private course
work, no personal email address.
