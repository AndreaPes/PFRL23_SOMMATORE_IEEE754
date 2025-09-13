# IEEE 754 Floating-Point Adder
Politecnico di Milano — Reti Logiche — _AY 2022–2023_

## About
Design and implementation of a pipelined IEEE 754 floating-point adder in VHDL.  
Handles normalized/denormalized operands and special values (NaN, ±Infinity, signed zero). Verified with dedicated testbenches across nominal and edge cases.

Deliverables:
- **VHDL sources**
- **Testbenches**
- **Project report**

## Goal and requirements
- Conform to IEEE 754 semantics for addition, including special-case handling.  
- Align → add/subtract → normalize → round (nearest-even) pipeline.  
- Detect and flag exceptional conditions (overflow/underflow, invalid ops).  
- Balance **latency** and **throughput** via pipelining.  
- Provide deterministic, reproducible simulations via testbenches.

## Key learnings
- **IEEE 754 semantics:** representation, special values, rounding, exception flags.  
- **Microarchitecture:** align/add/normalize/round (AANR) with clear stage boundaries.  
- **Pipelining:** partition logic to meet timing while preserving correctness.  
- **Verification:** craft directed and random tests for corner cases and regression.  
- **Synthesis & timing:** reason about critical paths, area vs. frequency trade-offs.  
- **Teamwork:** split design/verification tasks, review RTL/test code, and iterate.

## Team Members
- [Andrea Pesciotti](https://github.com/AndreaPes)
- [Domenico Pittari](https://github.com/Clav3rbot)

## License
This project is licensed under the [Apache License 2.0](./LICENSE).
