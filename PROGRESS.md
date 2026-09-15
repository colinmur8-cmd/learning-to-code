# Progress log

Newest entry at the top. Each entry: what we covered, what CS concept it
mapped to, what's next.

---

## 2026-09-15 — First program: implied probability

Colin has never written a line of code before this session. Started from
absolute zero, no assumed knowledge.

- Covered: sequential execution (program counter / top-to-bottom
  instruction order), variables as named memory locations, mutable state
  on reassignment, arithmetic operators, `NameError` from Python's
  exact-match name lookup (typos aren't "close enough"), and data types
  (`int` vs `float`, Python 3's true-division behaviour vs. other
  languages' silent-truncating integer division).
- Colin wrote (with guided correction, not dictation) a working 3-line
  program computing implied probability from decimal odds — saved at
  `projects/01-beginner/probability.py`.
- Deliberately flagged which parts were "software engineering fundamentals"
  (types, division semantics, exact lookups) vs. "domain math" (the
  1/odds formula itself), per his instructions.
- **Next session:** overround calculation — sum of implied probabilities
  across a market's outcomes minus 1. Naturally motivates **lists** (to
  hold multiple odds) and **loops** (to avoid copy-pasting the same
  calculation per outcome). Ask what he thinks the approach should be
  before introducing either concept.

---

## 2026-09-15 — Repo setup

- Scaffolded the repo: `CLAUDE.md` (mentor rules for future sessions),
  `README.md`, `PROGRESS.md`, and stub folders for the project ladder
  (`projects/01-beginner` through `05-engineering-practice`).
- No project code written yet — nothing to teach against until Colin picks
  a starting point.
- **Next session:** confirm which stage to start at (default: `01-beginner`,
  implied-probability/overround calculator from betting odds) and whether
  Colin wants to attempt a first pass himself before any concept is taught.
