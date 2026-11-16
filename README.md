# Tier 1 · Mathematical Thinking · Submissions

**Programme:** Mathematics for Computing, a self-study track (MC 001 to MC 350)
**Tier 1:** Mathematical Thinking: MC 100, MC 110, MC 120 · Mon 9 Aug 2027 to Sun 23 Jan 2028

This repository holds everything submitted for Tier 1: one answer sheet per graded item, and the Java code written
for each lab. Every tier of the track has its own repository, as every CSE semester does.

---

## Courses

| Folder | Course | When | Status | Sheets | Variable |
|---|---|---|---|---|---|
| `0. MC 100/` | MC 100 Logic, Sets and Proof | Mon 9 Aug 2027 – Sun 3 Oct 2027 | complete | 22 | `$MC100` |
| `1. MC 110/` | MC 110 Discrete Mathematics | Mon 4 Oct 2027 – Sun 12 Dec 2027 | complete | 28 | `$MC110` |
| `2. MC 120/` | MC 120 Computer Arithmetic and Boolean Algebra | Mon 13 Dec 2027 – Sun 23 Jan 2028 | complete | 13 | `$MC120` |

Each course folder has a README with its weeks, its topics and its sheets, then `week1/`, `week2/`, …, one per teaching
week. A week's sheets appear once its material is written, so a planned course holds only its README for now. Course
material for this tier is in the vault under `1. Tier 1 - Mathematical Thinking/`.

---

## How each assessment is submitted

1. Write the answer under each heading of the answer sheet. Lab code goes in the same `weekN/` folder, and the
   sheet's **Code:** line names the files.
2. Fill in *Help I Used* and set `status: submitted` in the frontmatter.
3. Commit and push **from this folder** (it's the repository, not the vault):
   ```bash
   cd "$MC100/.."      # any course variable of this tier, then up one level
   git add -A && git commit -m "MC NNN Week N: Practice N, Lab N, Quiz N submitted" && git push
   ```
4. After grading, the sheet's `score:` is filled in, `status:` becomes `graded`, and
   `python3 tools/gpa.py --sync --write` (from the vault's `9. Track Registry/`) copies it to the gradebook.

---

## What is ignored

- `.gitignore` at the repo root applies to every course: Obsidian state, OS and editor files, Python bytecode and
  compiled Java (`*.class`). The labs run from source with `java Lab.java`, so nothing compiled needs keeping.
- The last rule, `practice/`, ignores every week's practice folder. Experiments and test code stay local, so anything
  meant for grading goes in `weekN/` itself.

---

*Tier 1 · Mathematics for Computing · `ZerosAndOnesGlover/mc-tier1-mathematical-thinking`*
