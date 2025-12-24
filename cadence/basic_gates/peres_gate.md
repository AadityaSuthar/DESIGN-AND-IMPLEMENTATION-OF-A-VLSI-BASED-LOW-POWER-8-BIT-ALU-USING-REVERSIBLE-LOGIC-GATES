# Peres Gate

The Peres gate is a 3×3 reversible logic gate that efficiently combines the
functions of the Feynman and Toffoli gates into a single structure. It is widely
used in reversible arithmetic circuits due to its reduced gate count and lower
number of garbage outputs.

## Input–Output Relationship
- Inputs: A, B, C
- Outputs:
  - P = A
  - Q = A ⊕ B
  - R = (A · B) ⊕ C

## Importance in Reversible Design
The Peres gate provides both XOR and AND-related functionality in one gate,
making it highly suitable for arithmetic operations such as addition.

## Role in This Project
In this project, the Peres gate is implemented at the transistor level using
transmission-gate-based logic in Cadence Virtuoso. It is used as the primary
building block for designing the reversible full adder, which forms the core
of the 8-bit ALU.
