# Quantum Trajectory Cloning Cost

**Can a quantum processor reproduce a measured trajectory twice while retaining its original outcome probabilities?**

This project studies a labeled pure-state source, the physical two-copy conditional output, and the copy cost of knowing only the probability multiset versus knowing its assignment to labels.

**Established baseline:** a repeat-label protocol reproduces the full target exactly using **M + 1 expected source copies** for any full-support distribution on M labels. Its hard-budget failure tail is explicitly bounded.

**Research frontier:** a proposed linear-versus-square-root separation between hidden and known probability assignments. The universal converse and the known-assignment square-root construction are **not yet proved**; the proposed separation must not be cited as an established theorem.

## Read the project

- [Operational model and proposed claim](science/model.md)
- [Exact repeat-label construction and proof obligations](science/analysis.md)
- [Closest work and priority boundary](references/RELATED_WORK.md)
- [Verification plan](verification/README.md)
- [Watrous (2018) educational bridge](learning/WATROUS_BRIDGE.md)
- [30-milestone learning map](learning/MILESTONES.md)

The single educational anchor is John Watrous, *The Theory of Quantum Information* (2018). The milestone map is shared learning material; personal coaching and learner progress are not stored here.

## Scope and contact

The source supplies copies of an unknown coherent pure state, not a preparation oracle. The target includes the classical label and two conditional quantum specimens, and the performance metric is unconditional half trace distance. No gate-efficiency or hardware claim is made.

This repository serves as a record of the work and a guide for the author’s self-directed learning. For discussion or potential collaboration, please contact Ruge Lin at [gogoko699@gmail.com](mailto:gogoko699@gmail.com).
