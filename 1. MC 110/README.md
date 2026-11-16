# MC 110 · Discrete Mathematics

**Course:** MC 110, Discrete Mathematics (Tier 1, 10 weeks)
**When:** Mon 4 Oct 2027 – Sun 12 Dec 2027 · **Status:** complete
**Course material:** `1. Tier 1 - Mathematical Thinking/1. MC 110 - Discrete Mathematics/`
**Shell variable:** `$MC110` (defined once from *Shell variables* in the vault's `9. Track Registry/4. Submissions/README.md`)

Computers deal in separate, countable things: bits, keys, records, nodes, steps. This course is the maths of those
things. It counts them without listing them (how many passwords, how many paths, how many ways a hash can collide),
defines things in terms of smaller copies of themselves and solves the recurrences that recursive code produces,
connects things with relations and graphs, and ends with arithmetic on a clock, which is where modern cryptography
lives. MC 100 gave you the tools: proof by induction, by contradiction, by cases, and the habit of writing a reason
for every step. Here they get used every week, on new objects.

**Needs:** MC 100. **Unlocks → CSE:** MATH 151, CS 102 (recurrences, graphs), CS 301, CS 341 (RSA).

This folder holds everything submitted for MC 110: one answer sheet per graded item, and the Java code written for
each lab, side by side in the week it belongs to.

---

## Weeks

| Week | Dates | Topic | Sheets |
|---|---|---|---|
| 1 | Mon 4 – Sun 10 Oct 2027 | Count without listing: add for "or", multiply for "and then". | Lab 1 · Practice 1 · Quiz 1 |
| 2 | Mon 11 – Sun 17 Oct 2027 | Choosing, not arranging; and why some collisions can't be avoided. | Lab 2 · Practice 2 · Quiz 2 |
| 3 | Mon 18 – Sun 24 Oct 2027 | Correct for double counting; share identical things out. | Lab 3 · Practice 3 · Quiz 3 |
| 4 | Mon 25 – Sun 31 Oct 2027 | Define a thing by a smaller copy of itself. | Lab 4 · Practice 4 · Quiz 4 |
| 5 | Mon 1 – Sun 7 Nov 2027 | Closed forms for Fibonacci, and the running time of divide and conquer. | Lab 5 · Practice 5 · Quiz 5 |
| 6 | Mon 8 – Sun 14 Nov 2027 | Which things are related to which, and what "the same" means. | Lab 6 · Practice 6 · Quiz 6 |
| 7 | Mon 15 – Sun 21 Nov 2027 | Dots and lines: the shape of every network. | Lab 7 · Practice 7 · Quiz 7 |
| 8 | Mon 22 – Sun 28 Nov 2027 | Walk every edge, visit every vertex, colour the map. | Lab 8 · Practice 8 · Quiz 8 |
| 9 | Mon 29 Nov – Sun 5 Dec 2027 | Arithmetic on a clock, and how to divide there. | Lab 9 · Practice 9 · Quiz 9 |
| 10 | Mon 6 – Sun 12 Dec 2027 | A lock anyone can close and only you can open. | Final |

A week's sheets appear when its material is written (`tools/make_sheets.py`), so a week marked *awaiting material*
is empty for now. Dates after August 2027 are provisional (CALENDAR).

---

## Assessment

**Weights:** Practice 40% (lowest dropped) · Labs 20% · Quizzes 15% (lowest dropped) · Final 25%.
**Sheets so far:** 28 (Practice 9 · Lab 9 · Quiz 9 · Final 1).

Each sheet's `assessment:` and `possible:` join it to its row in `2. Gradebook/1 Tier1 Mathematical Thinking/MC 110.md`. Don't
rename the files or edit those two fields.

---

## Where the code goes

```bash
cd "$MC110/week1"                 # already made, with its sheets; the lab's Setup block names the week
java Lab.java                     # Java 25 compact source files, run in place
```

Every `weekN/` folder is created together with its answer sheets when that week is built, so there is nothing to
`mkdir`. Write the lab's `.java` files **in the week folder itself**, beside `Lab N.md`, and name them on the sheet's
**Code:** line. Anything you only try out goes in `weekN/practice/`, which git ignores. Compiled `*.class` files are
ignored too.

---

*MC 110 · Mathematics for Computing · Submissions*
