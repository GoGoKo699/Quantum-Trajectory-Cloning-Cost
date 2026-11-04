# From Watrous (2018) to trajectory reproduction

**Single educational anchor:** John Watrous, *The Theory of Quantum Information* (2018), [complete text](https://jhwatrous.github.io/TQI.pdf).

Use the treatment of quantum states, channels, measurements and instruments (Chapters 1–2), trace norm and discrimination (Chapter 3), and symmetric-subspace/copy methods (Chapter 7) as foundations. The exact section numbering should be checked against the linked edition before attaching narrower pointers.

A project trajectory is an instrument outcome: measuring (A) gives classical (z) with probability (p_z) and normalized postmeasurement state (|psi_zangle). The **subnormalized** branch (p_z|psi_zanglelanglepsi_z|) is linear in the source density matrix; normalizing a branch separately is not. The output target must preserve these weights, rather than optimize only branchwise fidelity.

Watrous's trace norm provides the operational error: (D(ho,sigma)=	frac12|ho-sigma|_1) bounds the change in probability of any effect. This is what lets an output observable serve as a lower-bound witness. His channel framework also permits arbitrary coherent processing, so a proof against only sample-and-retry algorithms is not a universal converse.

**Worked example.** Let (M=2), (p=(1/4,3/4)), and conditional states (|0angle,|+angle). The desired output is a classical mixture of (|0angle_Z|00angle) with weight (1/4) and (|1angle_Z|++angle) with weight (3/4). A pair obtained by matching two independently measured labels is biased toward the second label: the unnormalized weights are (1/16) and (9/16). This is why collision detection alone does not reproduce the source distribution.

The textbook supplies the language and general inequalities, **not** the proposed linear copy lower bound. The project-specific task, exact repeat-label construction, and any future sharp converse must be derived and credited separately.
