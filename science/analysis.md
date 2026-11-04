# Exact construction and unresolved separation

## Exact repeat-label protocol

Measure the label on the first source copy, obtaining \(z\) and retaining its conditional qubit. Measure labels on fresh independent source copies until \(z\) reappears, and retain that qubit. Return the original label and both retained qubits. Given \(z\), the number of additional copies is geometric with mean \(1/p_z\). The first label has distribution \(p_z\), so the returned state is **exactly**
\[
\sum_z p_z|z\rangle\langle z|\otimes
|\psi_z\rangle\langle\psi_z|^{\otimes2}.
\]
For full support, the expected number of source copies is
\[
1+\sum_z p_z\frac1{p_z}=M+1.
\]
On the two-level family, a hard budget of \(1+t\) copies has abort probability
\[
\sum_zp_z(1-p_z)^t\le e^{-t/(2M)}.
\]
Returning an arbitrary normalized state on abort changes the target by trace distance at most that abort probability. This establishes an \(O(M)\) upper bound for fixed error without any probability assignment.

## Why collision-only selection is biased

Two independent label measurements match at \(z\) with probability \(p_z^2\). Conditioned on a match, the label law is \(p_z^2/\sum_jp_j^2\), not \(p_z\). A birthday collision procedure therefore needs a valid probability-dependent correction, and its total cost must include failed corrections. Knowing only the multiset of probabilities does not identify the needed per-label correction.

## Decisive missing proofs

The proposed linear lower bound requires a quantitative indistinguishability or channel-duality argument for **all** \(k=o(M)\), permitting arbitrary collective quantum processing and fixed trace error. Matching low-order input moments alone cannot establish it. A complete known-assignment square-root construction must be explicitly specified and checked as a quantum channel, including both conditional outputs and the label law. Finite-dimensional experiments are diagnostics, not a substitute for either uniform proof.

**Verified:** exact repeat-label output, \(M+1\) expected copies, hard-budget tail. **Unverified:** universal \(\Omega(M)\) converse, \(\Theta(\sqrt M)\) known-assignment law, and the proposed separation's novelty relative to primary literature.
