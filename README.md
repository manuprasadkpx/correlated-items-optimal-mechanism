
# Optimal Mechanism Design for Two Correlated Items

## 1. The Problem

Selling two items together or separately is not always straightforward when buyers' valuations for the items are correlated.

A seller must decide how to design the available purchasing options and set their prices to maximise expected revenue. The seller may offer each item separately, sell both items as a bundle, or introduce more complex options that allow buyers to purchase combinations of the items.

The central problem in this research is to understand how the relationship between the two valuations affects the revenue-maximising selling mechanism.

In particular, the study investigates whether simple deterministic mechanisms, such as separate pricing and bundling, can achieve optimal revenue, or whether more complicated mechanisms involving lotteries can generate higher revenue.

## 2. The Unsolved Issue

Although mechanism design has established important results for independent valuations, extending these results to correlated valuations is considerably more challenging.

The main difficulty is proving global optimality.

Finding prices that maximise revenue within a particular class of deterministic mechanisms does not necessarily establish that those prices are optimal among all possible mechanisms.

A complete solution requires stronger mathematical conditions. In particular, the optimality of a proposed mechanism must be supported by an appropriate duality or transport certificate.

The research therefore addresses an important unresolved question:

**Under what conditions on the correlation between valuations can deterministic selling mechanisms be established as globally optimal, and when might more complicated mechanisms be necessary?**

## 3. What Has Been Done

The study develops a two-item valuation model using the Farlie–Gumbel–Morgenstern copula to represent different degrees of dependence between the two valuations.

The work has progressed through several stages:

- Developed the joint valuation distribution and examined how changes in correlation affect the distribution of valuations.
- Derived the transformed revenue density used in the optimal transport analysis.
- Identified the parameter range in which the transformed density remains non-negative throughout the valuation space.
- Developed the revenue expressions for symmetric deterministic pricing and bundling.
- Derived and evaluated the first-order conditions for candidate optimal prices.
- Investigated the geometric structure of the allocation regions using exact integration and polygon-based computational methods.
- Examined first-order stochastic dominance conditions relevant to establishing deterministic mechanism optimality.
- Developed duality-based transport constructions for selected parameter regimes.
- Used numerical optimisation and linear programming to examine the feasibility of candidate optimality certificates.
- Tested whether introducing lottery-based purchasing options could improve upon the revenue obtained from deterministic mechanisms.

## 4. How the Problem Has Been Addressed

The research combines analytical derivations with computational verification.

First, the valuation model is used to derive the transformed revenue density. This helps identify the correlation range in which the proposed transport-based approach can be applied.

Second, deterministic pricing and bundling mechanisms are analysed. Their candidate prices and expected revenues are obtained through analytical optimisation and numerical evaluation.

Third, the study investigates whether the proposed mechanisms satisfy the conditions required for global optimality. This involves examining allocation regions, stochastic dominance, and transport-based duality conditions.

A particularly important part of the work is the construction of transport couplings for different allocation regions. These constructions provide a way to investigate whether the revenue-maximising deterministic mechanism can be supported by a valid optimality certificate.

Finally, computational tests are used to check the feasibility of the proposed conditions and to compare deterministic mechanisms with selected lottery-based alternatives.

The computational work is treated as a verification tool for the analytical arguments, rather than as a substitute for a mathematical proof.

## 5. Main Results So Far

### 5.1 Transformed density

The study identifies the correlation interval in which the transformed revenue density remains non-negative across the valuation space.

This gives an important restriction for the transport-based analysis. However, the interval should not be interpreted as a proven threshold separating deterministic and randomized optimal mechanisms.

### 5.2 Deterministic pricing and bundling

The study derives candidate optimal prices for symmetric deterministic pricing and bundling.

The numerical analysis produces the following results:

| Correlation parameter | Individual-item price | Bundle price | Expected revenue |
|---|---:|---:|---:|
| -0.50 | 0.686228 | 0.833988 | 0.565724 |
| 0.25 | 0.654791 | 0.879565 | 0.541675 |
| 0.50 | 0.642219 | 0.899184 | 0.534811 |
| 0.75 | 0.629820 | 0.919758 | 0.528712 |

These results describe the optimised deterministic pricing candidates. They do not, by themselves, establish global optimality over every possible mechanism.

### 5.3 Optimal transport analysis

The research develops transport-based arguments for establishing deterministic optimality.

A complete certificate has been obtained for the independent-valuation benchmark. The analysis has also developed coupling constructions and feasibility checks for positive correlation within the admissible density range.

At a correlation parameter of 0.60, the computational analysis reports a candidate individual-item price of approximately 0.637190, a bundle price of approximately 0.907371, and expected revenue of approximately 0.532276. The associated linear programming feasibility check is successful.

These findings provide support for the proposed approach, although the full analytical scope of the certificate must be distinguished from the numerical feasibility result.

### 5.4 Lottery-based mechanisms

The study also investigates whether lottery-based purchasing options can improve revenue.

Several numerical comparisons have been conducted for negative and positive correlation settings. The tested lottery alternatives did not produce a revenue improvement over the corresponding deterministic candidates.

This is encouraging evidence for the deterministic mechanisms examined. However, testing selected lottery configurations does not establish that every possible randomized mechanism is inferior.

### 5.5 An important unresolved computational issue

A recent analytical slice-dominance test produced negative dominance slack, including at zero correlation.

This conflicts with the previously obtained independent-valuation optimality certificate. Consequently, the test's sign convention, orientation, and restrictions need to be reconciled before its output can be interpreted as evidence against deterministic optimality.

A negative result from this particular test cannot, on its own, disprove the earlier certificate.

## 6. What Remains Unresolved

The main remaining challenge is to establish a complete and internally consistent optimality characterisation across the full range of admissible correlation parameters.

The outstanding tasks include:

- Reconciling the recent slice-dominance test with the existing independent-valuation certificate.
- Completing the analytical transport and duality arguments beyond the independently distributed benchmark.
- Establishing the precise parameter conditions under which deterministic mechanisms are globally optimal.
- Determining whether any correlation regimes genuinely require randomized mechanisms.
- Distinguishing numerical evidence from results supported by complete mathematical proofs.

## 7. Conclusion

This research investigates how correlation between two item valuations changes the design of revenue-maximising selling mechanisms.

It develops a valuation model, derives candidate deterministic pricing strategies, examines allocation geometry, and applies optimal transport and computational methods to investigate global optimality.

The results so far provide a structured analytical and computational framework for studying the problem. They establish important properties of the transformed density, produce optimised deterministic pricing candidates, and provide an optimality certificate for the independent-valuation benchmark.

The numerical experiments have also found no revenue improvement from the particular lottery alternatives tested.

However, the general question of deterministic optimality across the entire correlation range remains open. Further work is required to reconcile the latest dominance test and complete the transport-based proof.

**The central contribution of the project is therefore a systematic analytical and computational investigation of the conditions under which deterministic mechanisms can be optimal when valuations are correlated.**

---

## Keywords

Mechanism Design, Optimal Auctions, Correlated Valuations, FGM Copula, Optimal Transport, Revenue Maximisation, Stochastic Dominance, Duality, Deterministic Mechanisms, Randomised Mechanisms.
