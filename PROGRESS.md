# Progress log

Newest entry at the top. Each entry: what we covered, what CS concept it
mapped to, what's next.

---

## 2026-09-23 — Aligning to CS1117 lectures + conditionals

Colin asked to sync the pace of this repo to his actual UCC module,
**CS1117: Introduction to Programming**. Read his lecture PDFs (2:
Programming Overview, 3: Variables/Data Types/Operators, 4&5: Input/
Output, 6: Conditional Statements) to establish where the course
actually is.

- **Status check:** we were *ahead* of the course on loops/lists/
  accumulator (not covered in lectures yet — parked, not wasted) and
  *behind* on `input()` and conditionals (`if`/`elif`/`else`), which is
  the most recent lecture. Realigned to conditionals.
- Colin extended his own edge-percentage program (`shergar_odds` /
  `sher_trueodds` ratio) with an `if`/`else` to classify a bet as
  `"value"` or `"no value"`.
- Debugged through, in order: `IndentationError` from indenting a line
  with no preceding colon-ended header; `SyntaxError` from a missing
  colon after the `if` condition; a **semantic error** (program ran with
  no error but both branches printed the same message) — tied directly
  to his own lecture's syntactic-vs-semantic error distinction; and an
  indentation-consistency mismatch between the two branches (5 vs 4
  spaces), worked through literally space-by-space since it's hard to
  see in plain chat text.
- Saved as `projects/01-beginner/value_bet.py`.
- **Next session:** combine this with `input()` (lecture 4&5, not yet
  practiced) so the odds come from the user instead of being hardcoded —
  mirrors exactly how the lecture's own ExamMarks/Temperature-Warning
  examples work (input → cast → branch). After that, extend to `elif`
  for a 3-way case (e.g. value / fair / no value) once the course
  reaches loops, revisit the parked overround/accumulator work.

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
