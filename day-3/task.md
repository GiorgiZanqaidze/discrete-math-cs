# Day 03 — §1.2 Propositional Equivalences — Tasks

**Date:** March 18, 2026  
**Time:** 9:00–10:00 AM  
**Status:** 🔲 Not Done  

---

## Laws to Reference

| Law | Formula |
|-----|---------|
| De Morgan's | ¬(p ∧ q) ≡ ¬p ∨ ¬q |
| De Morgan's | ¬(p ∨ q) ≡ ¬p ∧ ¬q |
| Double Negation | ¬(¬p) ≡ p |
| Commutative | p ∧ q ≡ q ∧ p / p ∨ q ≡ q ∨ p |
| Associative | (p ∧ q) ∧ r ≡ p ∧ (q ∧ r) |
| Distributive | p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r) |
| Distributive | p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r) |
| Conditional | p → q ≡ ¬p ∨ q |
| Contrapositive | p → q ≡ ¬q → ¬p |

---

## Set A — Apply De Morgan's (negate and simplify)

### #1
**Expression:** ¬(p ∧ q)  
**My answer:**  ¬p ∨ ¬q


### #2
**Expression:** ¬(¬p ∨ q)  
**My answer:**  p ∧ ¬q


### #3
**Expression:** ¬(p ∧ (q ∨ r))  
**My answer:**  ¬(p ∧ q) ∧ ¬(p ∧ r)


---

## Set B — Prove Equivalence Using Laws (name each law, no truth tables)

### #4
**Prove:** p → q ≡ ¬q → ¬p  
**My proof:**  
Step 1:  p → q === ¬p ∨ q ; ¬q → ¬p === q ∨ ¬p conditionaldisjunction equivalence
Step 2:  ¬p ∨ q === q ∨ ¬p 
Step 3:  ¬p ∨ q === ¬p ∨ q


### #5
**Prove:** ¬(p → q) ≡ p ∧ ¬q  
**My proof:**  
Step 1:  ¬(¬p ∨ q) === p ∧ ¬q conditionaldisjunction equivalence
Step 2:  p ∧ ¬q === p ∧ ¬q
Step 3:  


### #6
**Prove:** p ∨ (p ∧ q) ≡ p  (Absorption Law)  
**My proof:**  
Step 1:  (p ∨ p) ∨ (p ∧ q) === T ∨ (p ∧ q)
Step 2:  T ∨ (p ∧ q) === T Domination laws
Step 3:  


---

## Set C — Simplify to Shortest Form

### #7
**Expression:** (p ∧ q) ∨ (p ∧ ¬q)  
**Simplified:**  
**Laws used:**  


### #8
**Expression:** ¬(¬p ∧ ¬q)   
**Simplified:**  p ∨ q
**Laws used:**  De Morgan’s laws


### #9
**Expression:** (p → q) ∧ (q → p)  
**Simplified:**  p double conjunction with q
**Laws used:**  


---

## Corrections & Takeaways

_(fill in after grading)_
