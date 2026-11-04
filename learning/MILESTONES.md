# Thirty-milestone understanding map

The map has 12 foundational milestones and 18 research milestones. Each milestone is a common understanding target, not a record of personal coaching.

## Background and preliminaries (M01–M12)

| ID | Central question and understanding target | Dependency / source |
|---|---|---|
| M01 | What is a quantum state? Distinguish a state vector from its density operator. | Watrous Ch. 1 |
| M02 | What does an independent source copy mean? Interpret tensor products and copy budgets. | M01; Watrous Ch. 1 |
| M03 | How does a projective measurement work? Compute outcome probabilities. | M01; Watrous Ch. 2 |
| M04 | What survives a measurement? Normalize a conditional postmeasurement state. | M03; Watrous Ch. 2 |
| M05 | What is an instrument? Keep classical outcomes and quantum branches together. | M04; Watrous Ch. 2 |
| M06 | Why are branch weights essential? Contrast conditional and unconditional correctness. | M05; science/model.md |
| M07 | What is a quantum channel? Recognize arbitrary coherent processors and ancillas. | M02,M05; Watrous Ch. 2 |
| M08 | What is trace distance? Connect its norm to distinguishable measurement statistics. | M07; Watrous Ch. 3 |
| M09 | Why does no-cloning matter? Separate unknown-state duplication from retaining two originals. | M02,M07; related work |
| M10 | What is a collision? Compute repeated-label probabilities and size bias. | M03,M06; science/analysis.md |
| M11 | What is a copy lower bound? Distinguish restricted algorithms from all channels. | M07–M10; Watrous Ch. 3 |
| M12 | How do these ingredients define the task? State the target, input and accuracy together. | M01–M11; science/model.md |

## Research narrative (M13–M30)

| ID | Central question and understanding target | Dependency / source |
|---|---|---|
| M13 | What is the target ensemble? Write its labeled two-copy density operator. | M12; model |
| M14 | What is unknown? Separate probability multiset, assignment and conditional states. | M13; model |
| M15 | What is the hard two-level family? Check normalization and probability ratio. | M14; model |
| M16 | How can two genuine specimens be obtained? Follow the repeat-label protocol. | M10,M15; analysis |
| M17 | Why is the output distribution correct? Derive the first-label law. | M16; analysis |
| M18 | What is its expected cost? Sum the geometric waiting times. | M17; analysis |
| M19 | How does a hard budget work? Bound the abort probability and trace error. | M18; analysis |
| M20 | What goes wrong with first collisions? Derive the squared-probability bias. | M10,M15; analysis |
| M21 | What could known probabilities enable? Identify the required bias correction. | M20; analysis |
| M22 | Why is a birthday bound not enough? Distinguish collision frequency from output correctness. | M21; analysis |
| M23 | What must a universal converse allow? Enumerate joint quantum strategies. | M11,M22; analysis |
| M24 | How can output distinguishability yield a lower bound? Design an observable witness. | M08,M23; analysis |
| M25 | Why are matching second moments insufficient? Identify the missing all-copy estimate. | M24; analysis |
| M26 | What does a Choi optimization test? Interpret finite-copy channel feasibility. | M23; verification |
| M27 | What is a matching construction? Charge selection, correction and all failures. | M21,M26; verification |
| M28 | What belongs to earlier work? Separate no-cloning, collisions and this proposed law. | M09,M27; related work |
| M29 | Which claims are proved and open? Audit constants, quantifiers and assumptions. | M13–M28; analysis |
| M30 | What would complete the contribution? Synthesize matching proofs, implementation and significance. | M29; model, verification |
