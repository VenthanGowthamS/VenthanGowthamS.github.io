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

## The log

A dated timeline below the hero covers books finished, speeches, runs, builds, learning and work. It's a diary and a showcase at once, and visitors can filter it. Add entries to `LOG` in `index.html`; newest-first sorting is automatic.

## Archive

**`/archive/`** shows every past version with a screenshot and the idea behind it: Terminal → Orb → 2050 → 3100 → 2126. Each one still runs at its own path (`/terminal/`, `/orb/`, `/2050/`, `/3100/`).

## How it's built

- Plain HTML, CSS and JavaScript in one file per page: no framework, no build step, no backend.
- The core is about 2,200 points on a 2D canvas, with a hand-built 3D projection and lighting. Rendering pauses when the hero is off screen, and it respects the "reduce motion" setting.
- The console answers from facts written in the page.
- Valid HTML, with zero axe accessibility violations. It has link-preview tags, so it shares well on LinkedIn.

## Update content

Everything lives near the top of `index.html`'s script:

| What | Where | Notes |
|---|---|---|
| Books | `BOOKS` | `lang`, `done: 'YYYY-MM'`, `reading: true`, `cover: 'books/<name>.jpg'` (about 480px wide, under 100 KB) |
| Speech notes | `SECTIONS` → `speak` items | add `date: 'YYYY-MM'` and `notes: '…'`; they show as a "My notes" layer |
| Videos | `VIDEOS` | YouTube IDs; videos play inline on the site |
| Log | `LOG` | `{date, type: book/speech/run/build/learn/work, title, note, open}` |
| Links | `LINKS` | `linkedin`, `youtube` |

Each item has `s` (plain one-liner), `i` (why it matters), `m` (under the hood), `d` (the story) and optional `l` (links).

**Why videos aren't stored in this repo:** GitHub rejects files over 100 MB, Pages sites should stay under 1 GB, and Pages doesn't stream video well. YouTube (public or unlisted) streams to any phone at the right quality for free, and the site embeds it.

What's still needed from me is in [TODO.md](TODO.md).

## Custom domain (later)

Add a `CNAME` file containing the domain, point the domain's DNS at GitHub Pages, then turn on "Enforce HTTPS" in Settings → Pages.
