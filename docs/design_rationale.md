# Design Rationale and Gate Selection

## Why Reversible Logic?
Conventional logic circuits lose information during computation, which leads
to energy dissipation as described by Landauer’s principle. Reversible logic
preserves information by maintaining a one-to-one mapping between inputs and
outputs, making it attractive for low-power and future computing paradigms.

## Quantum Computing Relevance
Quantum computation inherently requires reversible operations. Classical
reversible logic gates form the foundation for quantum logic gates, making
reversible gate-based designs conceptually aligned with quantum systems.

## Gate Selection Rationale
- **Feynman Gate**: Used for signal copying and inversion, essential because
  fan-out is not allowed in reversible logic.
- **Toffoli Gate**: Acts as a universal reversible gate and is useful for
  controlled operations.
- **Fredkin Gate**: Provides conditional swapping functionality, useful in
  control logic.
- **Peres Gate**: Combines the functionality of Feynman and Toffoli gates,
  making it efficient for arithmetic circuits such as adders.

## Impact on ALU Design
These gates were chosen to minimize garbage outputs and gate count while
maintaining reversibility. The Peres gate was primarily used in the reversible
full adder design, which forms the core building block of the 8-bit ALU.
