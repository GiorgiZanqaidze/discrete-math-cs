# Day 03 — §1.2 Propositional Equivalences — Tasks

**Date:** March 18, 2026  
**Time:** 9:00–10:00 AM  
**Status:** ✅ Done  
**Score:** 5/9  

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
| Identity | p ∧ T ≡ p / p ∨ F ≡ p |
| Domination | p ∨ T ≡ T / p ∧ F ≡ F |
| Negation | p ∨ ¬p ≡ T / p ∧ ¬p ≡ F |
| Idempotent | p ∨ p ≡ p / p ∧ p ≡ p |

---

## Set A — Apply De Morgan's (negate and simplify) — 2/3

### #1 ✅
**Expression:** ¬(p ∧ q)  
**My answer:**  ¬p ∨ ¬q


### #2 ✅
**Expression:** ¬(¬p ∨ q)  
**My answer:**  p ∧ ¬q


### #3 ❌
**Expression:** ¬(p ∧ (q ∨ r))  
**My answer:**  ¬(p ∧ q) ∧ ¬(p ∧ r)  
**Correct answer:** ¬p ∨ (¬q ∧ ¬r)  
**Why wrong:** De Morgan's works one layer at a time. First flip ∧ to ∨ and negate the two operands: ¬p ∨ ¬(q ∨ r). Then apply De Morgan's again to ¬(q ∨ r): ¬p ∨ (¬q ∧ ¬r). Don't try to distribute across the whole expression at once.


---

## Set B — Prove Equivalence Using Laws (name each law, no truth tables) — 2/3

### #4 ✅
**Prove:** p → q ≡ ¬q → ¬p  
**My proof:**  
Step 1:  p → q ≡ ¬p ∨ q *(Conditional equivalence)*  
Step 2:  ¬p ∨ q ≡ q ∨ ¬p *(Commutative law)*  
Step 3:  q ∨ ¬p ≡ ¬(¬q) ∨ ¬p ≡ ¬q → ¬p *(Double negation + Conditional equivalence)*


### #5 ✅
**Prove:** ¬(p → q) ≡ p ∧ ¬q  
**My proof:**  
Step 1:  ¬(p → q) ≡ ¬(¬p ∨ q) *(Conditional equivalence)*  
Step 2:  ¬(¬p ∨ q) ≡ ¬(¬p) ∧ ¬q *(De Morgan's)*  
Step 3:  ¬(¬p) ∧ ¬q ≡ p ∧ ¬q *(Double negation)*


### #6 ❌
**Prove:** p ∨ (p ∧ q) ≡ p  (Absorption Law)  
**My proof:**  
Step 1:  (p ∨ p) ∨ (p ∧ q) === T ∨ (p ∧ q)  
Step 2:  T ∨ (p ∧ q) === T Domination laws  
Step 3:  *(incomplete)*  
**Why wrong:** p ∨ p ≡ p (Idempotent law), NOT T. T only comes from p ∨ ¬p (Negation law).  
**Correct proof:**  
Step 1: p ∨ (p ∧ q) ≡ (p ∧ T) ∨ (p ∧ q) *(Identity law: p ≡ p ∧ T)*  
Step 2: (p ∧ T) ∨ (p ∧ q) ≡ p ∧ (T ∨ q) *(Distributive law — factor out p)*  
Step 3: p ∧ (T ∨ q) ≡ p ∧ T *(Domination law: T ∨ q ≡ T)*  
Step 4: p ∧ T ≡ p *(Identity law)*


---

## Set C — Simplify to Shortest Form — 1/3

### #7 ❌ (skipped)
**Expression:** (p ∧ q) ∨ (p ∧ ¬q)  
**Simplified:**  *(left blank)*  
**Correct answer:** **p**  
**Solution:**  
Step 1: (p ∧ q) ∨ (p ∧ ¬q) ≡ p ∧ (q ∨ ¬q) *(Distributive — factor out p)*  
Step 2: p ∧ (q ∨ ¬q) ≡ p ∧ T *(Negation law: q ∨ ¬q ≡ T)*  
Step 3: p ∧ T ≡ p *(Identity law)*


### #8 ✅
**Expression:** ¬(¬p ∧ ¬q)   
**Simplified:**  p ∨ q  
**Laws used:**  De Morgan's laws + Double negation


### #9 ❌ (right idea, wrong notation)
**Expression:** (p → q) ∧ (q → p)  
**Simplified:**  p double conjunction with q  
**Correct answer:** **p ↔ q**  
**Note:** "If and only if" / biconditional. The symbol is ↔. (p → q) ∧ (q → p) is literally the definition of p ↔ q.


---

## Corrections & Takeaways

### Key Mistakes

1. **p ∨ p ≡ p (Idempotent), NOT T**  
   T only comes from p ∨ ¬p (Negation law). This is a critical distinction.

2. **De Morgan's works one layer at a time**  
   For ¬(p ∧ (q ∨ r)): first flip the outer ∧ → ∨ and negate operands, then handle the inner expression separately.

3. **The "rewrite p as p ∧ T" trick**  
   Key technique for Absorption and factoring proofs. p ≡ p ∧ T (Identity law) lets you factor out common terms using Distributive law.

4. **p ↔ q is the biconditional symbol**  
   (p → q) ∧ (q → p) ≡ p ↔ q. Must memorize this.

### Rosen Reference
- Table 6 on page 29 — master list of all equivalences
- Example 7 on page 32 — step-by-step proof walkthrough (the template for Set B)
