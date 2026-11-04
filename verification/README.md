# Verification plan

The exact repeat-label protocol can be checked analytically for every full-support distribution. For (M=2), (p=(1/4,3/4)), its expected copies are (1+sum_zp_z/p_z=3). Collision-conditioned labels instead have probabilities (1/10,9/10), not (1/4,3/4).

Required independent checks before scientific release:

1. Enumerate small two-level assignments and compute exact target matrices and candidate witnesses.
2. Optimize finite-copy quantum channels through a Choi semidefinite program for small (M,k), without imposing measurement-first processing.
3. Prove a dimension-uniform (k=o(M)) input-ensemble bound, rather than extrapolating finite examples.
4. Implement the known-assignment square-root construction, including rejection and normalization, and verify the actual joint labeled output.
5. Verify primary literature and error/success conventions.

No automated run or numerical proof is claimed in this version.
