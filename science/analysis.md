# Mechanisms, verified baseline, and decisive open checks

## Exact repeat-label construction

On the first input, measure (A), obtaining label (z) and state (|psi_zangle). Retain that state. Independently measure subsequent copies until the same label appears, and retain its conditional qubit. Conditional on (z), the waiting count is geometric with mean (1/p_z). Consequently the output is exactly
[
sum_z p_z|zanglelangle z|otimes|psi_zanglelanglepsi_z|^{otimes2}.
]
The expected copy cost is
[
1+sum_z p_zrac1{p_z}=M+1
]
for full support. This is **stronger** than the coarse (1+2M) bound. For a hard budget of (1+t) copies, failure probability is (sum_zp_z(1-p_z)^tle e^{-t/(2M)}) on the two-level family. Returning an arbitrary valid state on failure gives trace distance at most that failure probability. No unknown quantum cloning occurs: both retained specimens are original conditional samples.

## Why knowing the probability assignment might help

A birthday-style method can find repeated labels among (O(sqrt M)) independently measured copies. But choosing a repeated label weights it roughly by (p_z^2), rather than (p_z). Correcting this size bias requires an acceptance rule depending on the actual label probability, and the rule must be applied coherently or classically without losing the required qubit outputs. A known probability **multiset** is insufficient for that rule unless one also identifies the assignment.

## Converse design and pitfalls

The proposed hard family should randomize both the high/low assignment and the conditional qubit states, and then compare the output witness with the exact (k)-copy input moments. One must rule out quantum collective estimation of the assignment more efficiently than classical sampling, not assume it away. In particular, two ensembles matching through second moments do **not** by themselves imply an (Omega(M)) bound for arbitrary (k). A rigorous proof needs a quantitative indistinguishability bound for all (k=o(M)), or an equivalent channel dual certificate. The witness must be sensitive to the required joint labeled two-copy state and robust to fixed trace error.

The best-known relevant comparator is *No Cloning of Quantum Ensembles* (Du et al.; verify full bibliographic details before release). It must receive explicit credit for the task and the generic no-cloning barrier. Also compare to quantum conditional-state learning and coherent collision constructions, which solve different access/output tasks.

## Sanity-check status

Proved here: exact repeat-label algorithm, its (M+1) expected cost and hard-budget error bound. Not yet established here: a universal linear lower bound, an actual known-assignment square-root algorithm, matching constants, or priority of the proposed separation. These remain blockers to advertising the proposed (Theta(M)) versus (Theta(sqrt M)) separation as a theorem.
