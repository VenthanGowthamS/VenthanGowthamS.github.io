# To do: what Venthan sends, what Claude adds

Send these in chat (photos and voice notes are fine) and they go straight onto the site. Everything lives in `index.html`.

## Waiting on you

- [ ] **LinkedIn profile URL.** It adds a "LinkedIn" button to the contact section and the console.
- [ ] **Books: one photo of each cover** (Tamil and English), plus the month you finished it. They go into `books/` and onto the shelf, the Read planet and the log. The shelf orders itself: reading now, then newest finished.
- [ ] **Speech notes, one per speech:** the date, what it was about, and your prep notes. They show as a "My notes" layer on each talk and as an entry in the log. Speeches waiting for notes:
  - [ ] How Mental Models Rewired My Life (Best Speaker)
  - [ ] Deep Work (Best Speaker, Citi Toastmasters)
  - [ ] Beyond Boundaries (inaugural address, Chapter Meeting #244)
  - [ ] Home, Heart, Horizon (President's welcome)
  - [ ] ELEVATE workshop (host, Dell Technologies Singapore)
  - [ ] International Speech Contest (judge, SINDA)
- [ ] **Runs:** the date and distance (and time, if you want). Each run becomes a log entry under "Runs".
- [ ] **Work activities** worth showing: the date and one line each.
- [ ] **Videos:** upload to YouTube (public or *unlisted*) and send the links. The video IDs go into `VIDEOS` in `index.html`, and the videos play right on the site.

## GitHub housekeeping (needs your login, about 2 minutes)

- [ ] **Hide old repos from your profile:** in each repo, go to **Settings → Danger Zone → Change visibility → Make private**, for **TestGIT**, **Appium** and **Dyson**.
- [ ] **Pin the best repos:** on your GitHub profile, click **Customize your pins** and choose agent-evals-lab, Pannaipuram, kaizen-folio, daybrief-agent, VenthanGowthamS.github.io and mobile-bdd-appium.
- [ ] **Delete the leftover `docs/readme-cleanup` branch** in mobile-bdd-appium and web-bdd-selenium. It's under Branches.

## Later

- [ ] **Custom domain:** add a `CNAME` file and set the DNS. See the README.
- [ ] **agent-evals-lab:** re-run the real model with `--k 5` after the shop fix, if you want fresh numbers. The current numbers are still valid.
- [ ] **daybrief-agent:** set `GEMINI_API_KEY` in `.env` and run it for real. Weather and news are verified working.

## Done

- [x] One site for 2126: core, planets, lenses, console, log, archive
- [x] Book: *The LinkedIn Playbook for Employees* (Nov 2026)
- [x] Life section updated: kids, yoga daily, shuttle, running, building with AI
- [x] agent-evals-lab: the refund policy is fully enforced, with 11 tests
- [x] daybrief-agent: weather for "Theni,IN" fixed, with 19 tests
