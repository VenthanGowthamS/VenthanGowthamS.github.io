# venthangowthams.github.io

My personal site: a digital self that evolves from Neanderthal to a 2050 interface. It covers what I build, how I evaluate AI agents, what I read, and where I speak.

**Live:** https://venthangowthams.github.io

## Three modes

| Mode | Path | Style |
|---|---|---|
| **2050** (default) | `/` | Colourless holographic interface with a light-particle human head that evolves Neanderthal → Homo sapiens → digital self |
| **Orb** | `/orb/` | Glowing orb avatar whose hands reach out to Build · Evaluate · Read · Speak · Watch |
| **Terminal** | `/terminal/` | Agent-terminal style, ask the twin by typing commands |

A switcher in the corner of every page moves between them.

## How it's built

- Plain HTML, CSS and JavaScript: no framework, no build step, no backend.
- The 2050 head is about 10,000 points drawn on a 2D canvas, with a hand-built 3D projection and per-point lighting.
- The "ask me" twin answers from a fixed set of facts written in the page.
- Hosted on GitHub Pages. Each page is a single self-contained file.

## Update content

All content lives in the data arrays near the top of each page's `<script>`: `REPOS`, `BOOKS`, `TALKS`, `VIDEOS` and `LINKS`. Add a YouTube video by putting its ID in `VIDEOS`, and it plays inline on this site.

## Custom domain (later)

Add a `CNAME` file containing the domain, point the domain's DNS at GitHub Pages, then turn on "Enforce HTTPS" in Settings → Pages.
