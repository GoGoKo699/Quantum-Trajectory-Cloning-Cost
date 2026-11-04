# Operational model and research claim

Let (A) be an (M)-dimensional label register and (B) a qubit. The unknown pure source is
[
|Psiangle_{AB}=sum_{z=1}^Msqrt{p_z}|zangle_A|psi_zangle_B,
qquad sum_zp_z=1.
]
The label measurement is fixed and public. The desired **unconditional, normalized** output is
[
T(Psi)=sum_z p_z|zanglelangle z|_Zotimes
(|psi_zanglelanglepsi_z|)^{otimes2}_{B_1B_2}.
]
A processor receives (k) independent copies of (|Psiangle); it may use arbitrary joint channels, ancillas, intermediate measurements, classical control and postselection, but **all** consumed copies and failures count. The target includes the label distribution: merely cloning a conditionally selected branch does not solve this task. The primary accuracy measure is (D(ho,T)=	frac12|ho-T|_1), without conditioning on a favorable output event. A separate heralded formulation must explicitly count success and unsuccessful trials.

## Proposed separation and its proof obligations

For even (M), consider probabilities in ({1/(2M),3/(2M)}), with exactly (M/2) of each. The multiset is public; the assignment to labels is hidden. Conditional qubit states are arbitrary. The proposed fixed-small-error law is (Theta(M)) copies when the assignment is hidden, versus (Theta(sqrt M)) when it is given. **This is a research proposition, not a verified theorem in this repository until the full universal converse and constructive upper bound are checked.**

The linear upper bound is immediate up to constants: measure one source to obtain (z), retain its qubit, and sample further copies until the same label reappears; output both qubits. Since (p_zge1/(2M)), expected total consumption is at most (1+2M), with exact target law. A fixed hard budget (O(Mlog(1/delta))) bounds the abort probability by (delta). This works without knowing the probabilities.

The square-root lower bound from collision/no-cloning arguments and the proposed **linear** lower bound require separate proofs: a classical two-point probability-testing argument alone does not rule out collective coherent processors. A complete converse must compare the actual (k)-copy quantum ensembles (not merely measured labels) and a physically measurable output witness, with uniform constants and the target error convention. The known-assignment square-root upper bound must provide a source-independent CPTP or heralded protocol, correct its selection bias and explicitly charge rejected attempts. Do not infer either statement from birthday collisions alone.

## Important boundaries

The input is a pure coherent source, not an oracle for its preparation. A source-dependent classical probability table changes the access model. The output is a labeled pair of **quantum states**, not a scalar expectation, a sample of labels, or two independent marginal ensembles. The constant-error threshold, success convention and whether the probability assignment is fully known must be held fixed across comparisons.
