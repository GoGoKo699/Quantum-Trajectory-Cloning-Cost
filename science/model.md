# Operational model and research proposition

Let \(A\) be an \(M\)-dimensional label register and \(B\) a qubit. The unknown pure source is
\[
|\Psi\rangle_{AB}=\sum_{z=1}^{M}\sqrt{p_z}|z\rangle_A|\psi_z\rangle_B,\qquad \sum_zp_z=1.
\]
Measuring the public label register produces \(z\) with probability \(p_z\) and conditional state \(|\psi_z\rangle\). The required unconditional output is
\[
T(\Psi)=\sum_z p_z|z\rangle\langle z|_Z\otimes
(|\psi_z\rangle\langle\psi_z|)^{\otimes2}_{B_1B_2}.
\]
A processor receives \(k\) independent source copies and may perform arbitrary collective channels, ancillas, adaptive measurements and classical control. Every consumed copy and unsuccessful attempt counts. Error is half trace distance \(D(\rho,T)=\frac12\|\rho-T\|_1\). A heralded success formulation requires a separate explicit success threshold.

## Proposed separation

For even \(M\), exactly half of the \(p_z\) are \(1/(2M)\) and half are \(3/(2M)\). The multiset is public, but its assignment to labels may be hidden. The proposed fixed-small-error copy law is \(\Theta(M)\) for hidden assignment and \(\Theta(\sqrt M)\) when the assignment is supplied. **The matching lower and upper bounds have not been established in this repository and this statement remains a research conjecture.**

A rigorous converse must rule out arbitrary coherent processing of the input copies, not just measurement-first sampling. A known-assignment square-root protocol must reproduce the *original* label probabilities and output two correct qubits, with all rejected trials charged. The exact linear-cost repeat-label protocol is proved in [analysis](analysis.md).

The task is not scalar expectation estimation, marginal ensemble generation, or access to a source-preparation oracle. The error and success conventions must be identical across both information models.
