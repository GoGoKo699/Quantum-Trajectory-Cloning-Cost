# Watrous bridge

**Single educational anchor:** John Watrous, *The Theory of Quantum Information* (2018), [full text](https://jhwatrous.github.io/TQI.pdf). Read its foundations of states, channels and measurements (Chapters 1–2), trace distance and discrimination (Chapter 3), and symmetric tensor methods (Chapter 7).

A measured trajectory is a classical outcome \(z\) with probability \(p_z\) and conditional quantum state \(|\psi_z\rangle\). The unnormalized branch \(p_z|\psi_z\rangle\langle\psi_z|\) is the natural linear object; the normalized conditional state alone loses the branch weight. The target doubles the conditional qubit but must retain that weight.

Trace distance \(D(\rho,\sigma)=\frac12\|\rho-\sigma\|_1\) bounds the difference in every measurement-event probability. A lower bound for arbitrary channels must use a quantum-input discrimination argument, not just classical sampling.

**Example:** for \(p=(1/4,3/4)\) and conditional qubits \(|0\rangle,|+\rangle\), the target assigns weights \(1/4\) and \(3/4\) to \(|0\rangle_Z|00\rangle\) and \(|1\rangle_Z|++\rangle\). Two-copy label collisions instead have unnormalized weights \(1/16\) and \(9/16\), hence normalized weights \(1/10\) and \(9/10\).

Watrous supplies the framework, not the conjectured linear copy converse. The exact repeat-label construction and any future separation proof belong to this project's own research account.
