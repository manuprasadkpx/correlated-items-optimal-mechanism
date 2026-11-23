
# Optimal Mechanism Design for Correlated Items

## Research Overview

This project investigates optimal mechanism design for the sale of two correlated items. It examines how the dependence structure between item valuations influences revenue-maximising mechanisms, with particular attention to deterministic mechanisms and the conditions under which their optimality can be established.

The analysis combines analytical characterisation with computational verification, drawing on the optimal transport approach to mechanism design.

## 1. Research Question

How does correlation between buyers' valuations affect the structure and optimality of revenue-maximising mechanisms for two items?

The project focuses on identifying parameter conditions under which deterministic mechanisms satisfy the relevant optimality conditions.

## 2. Valuation Model

The model uses the Farlie–Gumbel–Morgenstern (FGM) copula to represent dependence between two uniformly distributed item valuations.

The joint density is:

\[
f_\alpha(x,y)
=
1+\alpha(1-2x)(1-2y),
\]

where:

\[
(x,y)\in[0,1]^2,
\qquad
\alpha\in[-1,1].
\]

The parameter \(\alpha\) controls the dependence structure between the two valuations.

## 3. Transformed Revenue Density

The analysis derives the transformed density:

\[
g_\alpha(x,y)
=
3+\alpha(3-8x-8y+20xy).
\]

The non-negativity condition for this transformed density is satisfied over the full valuation square when:

\[
\boxed{
\alpha\in\left[-\frac{3}{7},\frac{3}{5}\right]
}
\]

This parameter interval provides an important analytical restriction for the subsequent mechanism-design analysis.

## 4. Main Analytical Directions

The project investigates:

- The relationship between valuation dependence and optimal mechanism structure.
- Conditions governing deterministic menu regions.
- First-order stochastic dominance conditions.
- The construction and analysis of bundle regions.
- Optimal transport and duality-based conditions for establishing mechanism optimality.
- Computational feasibility checks across different correlation parameters.

## 5. Computational Approach

The analytical results are supplemented by numerical and computational procedures.

The computational work examines parameter-dependent conditions, evaluates dominance restrictions, and investigates the feasibility of candidate optimality certificates.

The numerical analysis is intended to complement the theoretical derivations rather than replace them.

## 6. Research Scope

The current project focuses on the analytical structure of deterministic mechanisms and the conditions required to establish their optimality.

The repository intentionally does not reproduce every intermediate derivation, complete numerical output, or the full computational implementation.

## 7. Research Status

This is an ongoing research project. Analytical conditions, computational results, and interpretations may be refined as the investigation progresses.

## 8. Keywords

Mechanism Design · Optimal Auctions · Correlated Valuations · FGM Copula · Optimal Transport · Revenue Maximisation · Stochastic Dominance · Duality

---

*This repository documents an ongoing research investigation. Please refer to the individual research files for the specific assumptions, derivations, and computational results.*
