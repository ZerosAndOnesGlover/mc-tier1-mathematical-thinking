# MC 120 · Computer Arithmetic and Boolean Algebra

**Course:** MC 120, Computer Arithmetic and Boolean Algebra (Tier 1, 5 weeks)
**When:** Mon 13 Dec 2027 – Sun 23 Jan 2028 · **Status:** complete
**Course material:** `1. Tier 1 - Mathematical Thinking/2. MC 120 - Computer Arithmetic and Boolean Algebra/`
**Shell variable:** `$MC120` (defined once from *Shell variables* in the vault's `9. Track Registry/4. Submissions/README.md`)

This is what the hardware actually does. You've seen the symptoms: `Integer.MAX_VALUE + 1` goes negative, and
`0.1 + 0.2 != 0.3` (MC 001 L11). You've seen the logic: every truth table is a formula, and NAND alone can build all of
them (MC 100 L03). This course joins the two. It starts with Boolean algebra as something you can calculate with, finds
the simplest circuit for a truth table with a Karnaugh map, and builds a page of gates that adds two numbers. Then it
shows why that same adder subtracts, how hardware shifts, multiplies and divides, and how a 64-bit pattern holds a
fraction. It ends by measuring how far a rounded answer can be trusted.

**Needs:** MC 001, MC 100. **Unlocks → CSE:** ECE 110 (digital logic), CS 201 (organisation), PROG 101/201 (integers, bit operations), MATH 341 (floating point).

This folder holds everything submitted for MC 120: one answer sheet per graded item, and the Java code written for
each lab, side by side in the week it belongs to.

---

## Weeks

| Week | Dates | Topic | Sheets |
|---|---|---|---|
| 1 | Mon 13 – Sun 19 Dec 2027 | Logic you can calculate with, and a picture that simplifies it. | Lab 1 · Practice 1 · Quiz 1 |
| 2 | Mon 27 Dec 2027 – Sun 2 Jan 2028 | A page of gates that adds, and the trick that makes it subtract. | Lab 2 · Practice 2 · Quiz 2 |
| 3 | Mon 3 – Sun 9 Jan 2028 | When the odometer bites, and how hardware multiplies with shifts and adds. | Lab 3 · Practice 3 · Quiz 3 |
| 4 | Mon 10 – Sun 16 Jan 2028 | Fractions with a fixed point, then a floating one. | Lab 4 · Practice 4 · Quiz 4 |
| 5 | Mon 17 – Sun 23 Jan 2028 | How far a rounded answer can be trusted; and the whole course on one page. | Final |

A week's sheets appear when its material is written (`tools/make_sheets.py`), so a week marked *awaiting material*
is empty for now. Dates after August 2027 are provisional (CALENDAR).

---

## Assessment

**Weights:** Practice 40% · Labs 20% · Quizzes 15% · Final 25% (four items each, none dropped).
**Sheets so far:** 13 (Practice 4 · Lab 4 · Quiz 4 · Final 1).

Each sheet's `assessment:` and `possible:` join it to its row in `2. Gradebook/1 Tier1 Mathematical Thinking/MC 120.md`. Don't
rename the files or edit those two fields.

---

## Where the code goes

```bash
mkdir -p "$MC120/week1" && cd "$MC120/week1"     # the lab's own Setup block gives the right week
java Lab.java                                    # Java 25 compact source files, run in place
```

Write the lab's `.java` files **in the week folder itself**, beside `Lab N.md`, and name them on the sheet's
**Code:** line. Anything you only try out goes in `weekN/practice/`, which git ignores. Compiled `*.class` files are
ignored too.

---

*MC 120 · Mathematics for Computing · Submissions*
