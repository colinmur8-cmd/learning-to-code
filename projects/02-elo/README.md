# 02 — Early intermediate: Elo from scratch

**What this teaches:** mutable state across time steps, loops over
sequences of matches, a first real data structure decision (how do you
look up a team's current rating — list scan vs dict?), and simple OOP (a
`Team`/`Player` class holding state + behaviour vs. plain functions on a
dict). Unit testing an update rule against known expected values.

**Domain side (secondary):** the Elo update formula itself, K-factor
choice, expected-score formula. This is GAA/football specific tuning, not
CS — don't let getting the K-factor "right" substitute for understanding
why a dict beats a list scan here.

Not started yet — pick this up once `01-beginner` is solid and tested.
