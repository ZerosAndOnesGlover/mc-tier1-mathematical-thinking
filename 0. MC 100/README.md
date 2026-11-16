# MC 100 · Logic, Sets and Proof

**Course:** MC 100, Logic, Sets and Proof (Tier 1, 8 weeks)
**When:** Mon 9 Aug 2027 – Sun 3 Oct 2027 · **Status:** complete
**Course material:** `1. Tier 1 - Mathematical Thinking/0. MC 100 - Logic, Sets and Proof/`
**Shell variable:** `$MC100` (defined once from *Shell variables* in the vault's `9. Track Registry/4. Submissions/README.md`)

Tier 0 rebuilt every rule from a picture. This course turns pictures into **proofs**: arguments that hold in every case,
not just the ones you drew. It starts with the language proofs are written in, logic and sets, which is also the
language of every `if`, `&&`, loop and type you write. Then it takes the proof techniques one at a time (direct,
contrapositive, contradiction, cases, induction), each shown step by step before you try it, and ends with a proof that
some infinities are bigger than others. You wrote short arguments in every Explain half of Tier 0; this course shows you
how to make them watertight.

**Needs:** MC 030. **Unlocks → CSE:** MATH 151 (all), CS 101, CS 301 (theory of computation), CS 412 (formal methods), PROG 202 (logic programming).

This folder holds everything submitted for MC 100: one answer sheet per graded item, and the Java code written for
each lab, side by side in the week it belongs to.

---

## Weeks

| Week | Dates | Topic | Sheets |
|---|---|---|---|
| 1 | Mon 9 – Sun 15 Aug 2027 | A statement is true or false, and "if… then" is only false in one case. | Lab 1 · Practice 1 · Quiz 1 |
| 2 | Mon 16 – Sun 22 Aug 2027 | Statements that always agree, and how to say "for every" and "there is". | Lab 2 · Practice 2 · Quiz 2 |
| 3 | Mon 23 – Sun 29 Aug 2027 | A set is a bag with no order and no repeats, and logic is how you combine them. | Lab 3 · Practice 3 · Quiz 3 |
| 4 | Mon 30 Aug – Sun 5 Sep 2027 | A proof is a chain where every link has a reason. | Lab 4 · Practice 4 · Quiz 4 |
| 5 | Mon 6 – Sun 12 Sep 2027 | Prove it backwards, prove the opposite is impossible, or check every case. | Lab 5 · Practice 5 · Quiz 5 |
| 6 | Mon 13 – Sun 19 Sep 2027 | Knock over the first domino, show each knocks over the next. | Lab 6 · Practice 6 · Quiz 6 |
| 7 | Mon 20 – Sun 26 Sep 2027 | Pairing things up is how you count, even to infinity. | Lab 7 · Practice 7 · Quiz 7 |
| 8 | Mon 27 Sep – Sun 3 Oct 2027 | A proof is written for a reader. | Final |

A week's sheets appear when its material is written (`tools/make_sheets.py`), so a week marked *awaiting material*
is empty for now. Dates after August 2027 are provisional (CALENDAR).

---

## Assessment

**Weights:** Practice 40% (lowest dropped) · Labs 20% · Quizzes 15% (lowest dropped) · Final 25%.
**Sheets so far:** 22 (Practice 7 · Lab 7 · Quiz 7 · Final 1).

Each sheet's `assessment:` and `possible:` join it to its row in `2. Gradebook/1 Tier1 Mathematical Thinking/MC 100.md`. Don't
rename the files or edit those two fields.

---

## Where the code goes

```bash
cd "$MC100/week1"                 # already made, with its sheets; the lab's Setup block names the week
java Lab.java                     # Java 25 compact source files, run in place
```

Every `weekN/` folder is created together with its answer sheets when that week is built, so there is nothing to
`mkdir`. Write the lab's `.java` files **in the week folder itself**, beside `Lab N.md`, and name them on the sheet's
**Code:** line. Anything you only try out goes in `weekN/practice/`, which git ignores. Compiled `*.class` files are
ignored too.

---

*MC 100 · Mathematics for Computing · Submissions*
