# Day 02 — §1.1 English → Formulas

**Date:** March 17, 2026  
**Time:** 9:00–10:00 AM  
**Status:** 🔲 Not Done  

---

## Key Concepts

### The 3 Traps in English → Logic Translation

**Trap 1: "Unless" = "if not"**

"The server crashes **unless** the backup is running"  
= "If the backup is NOT running, then the server crashes"  
= ¬b → c  
= equivalently: b ∨ c

**Trap 2: "Only if" ≠ "if"**

- "p **if** q" means q → p (q is sufficient for p)
- "p **only if** q" means p → q (q is necessary for p)

Example: "You pass **only if** you study" = pass → study.  
You can study and still fail, but you can't pass without studying.

**Trap 3: Implicit grouping**

English doesn't use parentheses. You must figure out grouping from context:

- "The alarm triggers if the door opens and the system is armed" = (d ∧ a) → t
- "The alarm triggers if the door opens, and the system is armed" = (d → t) ∧ a

A comma can change the entire meaning.

---

## Exercises — Set A (Direct Translation)

Define your variables and write the formula.

| # | English Statement | Variables | My Formula | Correct? |
|---|-------------------|-----------|------------|----------|
| 1 | "The API returns an error unless the token is valid." | | | |
| 2 | "You can deploy only if all tests pass." | | | |
| 3 | "The page loads if and only if the CDN is reachable and the server is up." | | | |
| 4 | "The notification is sent if the user is online or if the priority is high." | | | |
| 5 | "The build fails unless the config exists and the dependencies are installed." | | | |

## Exercises — Set B (Bug Hunting)

Each formula has a mistake. Find it and fix it.

### #6
**English:** "Access is granted if the user is an admin or the request is internal."  
**Given formula:** a ∧ r → g  
**What's wrong?**  
My answer:  


**My corrected formula:**  


### #7
**English:** "The email is sent only if the user has opted in and the address is verified."  
**Given formula:** (o ∧ v) → e  
**What's wrong?**  
My answer:  


**My corrected formula:**  


### #8
**English:** "The cache is cleared unless it was updated in the last hour."  
**Given formula:** u → ¬c  
**What's wrong?**  
My answer:  


**My corrected formula:**  


---

## Rosen Textbook Exercises

§1.1 Exercises 23–35: _(fill in after completing Sets A & B above)_

---

## Corrections & Takeaways

_(fill in after grading)_
