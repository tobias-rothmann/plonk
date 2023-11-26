# Implementing PLONK according to the original paper in Rust

### Disclaimer
This is a concept implementation and not for use in real-world applications.

## Source Paper 
This implementation reffers to the original paper "PlonK: Permutations over Lagrange-bases for Oecumenical Noninteractive arguments of Knowledge" by Ariel Gabizon, Zachary J. Williamson, and Oana Ciobotaru. To be found at: https://eprint.iacr.org/2019/953.pdf

## Implementation
This implementation tries to mirror the original paper definition as close as possible. 

## The polynomial commitment scheme Trait
In order to support easy exchangable implementations of polynomial commitment schemes, for e.g. use in different plonk versions (DL-KZG-PLONK as SNARK without zero knowledge, PED-KZG-PLONK as zk-SNARK, FRI-PLONK as STARK), I define a polynomial commitment scheme trait upfront, which is implemented by every consruction-implementation. 
#### Done
