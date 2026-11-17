# AZ-900 Practice Exam

An offline-capable practice app for the Microsoft AZ-900 (Azure Fundamentals) exam, built like the ISSAP and ENSLD apps.

- **300 original scenario questions**, weighted to the AZ-900 skills outline (as of July 20, 2026):

  | Domain | Weight | Bank | Per full exam |
  |---|---|---|---|
  | 1. Describe cloud concepts | 25-30% | 84 | 14 |
  | 2. Describe Azure architecture and services | 35-40% | 114 | 19 |
  | 3. Describe Azure management and governance | 30-35% | 102 | 17 |

- **Full practice exam**: 50 questions, 45-minute timer, flag and review, scored at the end (the real pass mark is 700/1000, so aim for 75%+ here).
- **5-question test**: timed (5 min), scored at the end.
- **Quick practice / domain drills / missed questions**: 5, 10, 20, 50, or all at a time, unseen questions first, explanation after each answer.
- Exam or study mode for the full exam and 5-question test.
- Progress is saved in the browser, with backup and restore as copy-paste text.
- Installable as a home-screen app (PWA) and works offline after the first load.

The bank is written harder than the real exam on purpose: scenario stems, "BEST / MOST cost-effective / LEAST effort" wording, multi-select items, CLI, KQL, ARM, and policy snippets, and close distractors (private vs service endpoints, GZRS vs RA-GZRS, Policy vs RBAC vs locks, Service Health vs Resource Health). Every question has an explanation covering why the distractors are wrong. Option lengths are balanced so the longest answer is not a giveaway.

## Files

- `index.html`: the app
- `bank/d1.js` to `bank/d3.js`: the question bank, one file per domain (`{id, d, q, o, a, e}`; `a` is the index of the correct option, and options are shuffled at display time)
- `sw.js`, `manifest.webmanifest`, `icon-*.png`: offline support and app install

Host it with GitHub Pages (Settings → Pages → deploy from branch) or open `index.html` from any static web server.

Questions are original study material, not exam dumps.
