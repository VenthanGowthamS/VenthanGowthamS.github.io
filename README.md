# venthangowthams.github.io

My personal site, imagined for the year 2126.

**Live:** https://venthangowthams.github.io

## What it is

One page that works for everyone who visits:

- **The core:** a sphere of light that is my agent. It ripples when it speaks, and two halo rings orbit it.
- **The solar system:** my work orbits the core as seven planets: Build, Evaluate, Method, Read, Speak, Watch and Life.
- **Three lenses:** visitors choose **Everyone**, **Leader** or **Engineer** at the top, and every summary, one-liner and "at a glance" number changes to fit. Each item opens into three layers: *in plain words*, *why it matters* and *under the hood*.
- **Read it as a page:** scrolling down shows everything as a plain, readable page, so nobody has to explore to find the facts.
- **The console:** a terminal at the bottom that anyone can use. Type in plain words or tap a suggestion. Commands include `help`, `lens leader`, `orbic` and `clear`.

## Invented languages

- **Orbic:** a small word-language for 2126. Planet names carry an Orbic word (*sora* = build, *kesh* = test, *lio* = read, *tama* = speak), always with English beside it.
- **Ora:** "intent code", where you state what you mean, not how to do it. The site's "hi code" is written in Ora, and the console boots with it.

## Past versions

| Version | Path |
|---|---|
| 2050: holographic head that evolves | `/2050/` |
| 3100: first solar system | `/3100/` |
| Orb: glowing orb with reaching hands | `/orb/` |
| Terminal: agent terminal | `/terminal/` |

## How it's built

- Plain HTML, CSS and JavaScript in one file per page: no framework, no build step, no backend.
- The core is about 2,200 points on a 2D canvas, with a hand-built 3D projection and lighting. Rendering pauses when the hero is off screen, and it respects the "reduce motion" setting.
- The console answers from facts written in the page.
- Valid HTML, with zero axe accessibility violations. It has link-preview tags, so it shares well on LinkedIn.

## Update content

Everything lives in the `SECTIONS`, `BOOKS`, `GLANCE` and `LINKS` objects near the top of `index.html`'s script. Each item has `s` (plain one-liner), `i` (why it matters), `m` (under the hood), `d` (the story) and optional `l` (links).

## Custom domain (later)

Add a `CNAME` file containing the domain, point the domain's DNS at GitHub Pages, then turn on "Enforce HTTPS" in Settings → Pages.
