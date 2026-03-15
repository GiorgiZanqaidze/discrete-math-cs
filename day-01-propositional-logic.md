# Day 01 — §1.1 Propositional Logic

**Date:** March 16, 2026  
**Time:** 9:00–10:00 AM  
**Status:** 🔲 Not Done  

---

## Key Concepts

### What is a proposition?
A **proposition** is a declarative statement that is either **true (T)** or **false (F)**.

- ✅ "2 + 3 = 5" → proposition (T)
- ✅ "JavaScript is a compiled language" → proposition (F)
- ❌ "What time is it?" → not a proposition (question)
- ❌ "x + 1 = 5" → not a proposition (depends on x)

### The Five Logical Connectives

| Symbol | Name           | JS Equivalent | Meaning              |
|--------|----------------|---------------|----------------------|
| ¬p     | Negation       | `!p`          | "not p"              |
| p ∧ q  | Conjunction    | `p && q`      | "p and q"            |
| p ∨ q  | Disjunction    | `p \|\| q`    | "p or q"             |
| p → q  | Conditional    | —             | "if p then q"        |
| p ↔ q  | Biconditional  | `p === q`     | "p if and only if q" |

### The Conditional (→) — Truth Table

| p | q | p → q |
|---|---|-------|
| T | T | **T** |
| T | F | **F** |
| F | T | **T** |
| F | F | **T** |

**Key insight:** p → q is only false when p is true and q is false.  
**Analogy:** A promise. "If it rains, I'll bring an umbrella." You only break the promise when it rains AND you don't bring one.

### Operator Precedence (highest → lowest)

¬ → ∧ → ∨ → → → ↔

So `¬p ∧ q → r` means `((¬p) ∧ q) → r`

---

## Exercises — Set A (Truth values)

Given: **p = T, q = F, r = T**

| # | Expression | My Answer | Correct? |
|---|-----------|-----------|----------|
| 1 | ¬p ∨ q | | |
| 2 | p ∧ ¬q | | |
| 3 | p → q | | |
| 4 | ¬q → ¬p | | |
| 5 | (p ∨ q) ∧ (¬r) | | |

## Exercises — Set B (English → Formula)

| # | English Statement | My Formula | Correct? |
|---|-------------------|------------|----------|
| 6 | "The server is running and the database is connected." | | |
| 7 | "If the request is valid, then the API returns 200." | | |
| 8 | "The user is logged in or the page is public, but not both." | | |
| 9 | "If the cache is empty and the database is down, the app crashes." | | |
| 10 | "The test passes if and only if all assertions are true." | | |

---

## Rosen Textbook Exercises

§1.1 Exercises 1–21 (odd): _(fill in after completing Set A & B above)_

---

## Corrections & Takeaways

_(write what you got wrong and why after grading)_

---

## Diagnostic Note

From the pre-course quiz, I got Problem 3 wrong:
- Misread "owner OR (admin AND not locked)" as "(owner AND not locked) OR (admin AND not locked)"
- Root cause: didn't respect operator precedence in natural language → logic translation
- This is the skill Set B exercises are designed to fix
