# Implementation of Symmetric Multiprocessing dual core system  using MESI Cache Coherence  Protocol
Dual-core cache coherence system implementing the MESI (Modified, Exclusive, Shared, Invalid) protocol in SystemVerilog. Includes two direct-mapped 512KB caches with 2-word block size, write-back policy, and write-invalidate mechanism. Project for high-speed multiprocessor system design.

## Specifications
- 2x 512KB direct-mapped caches
- Block size: 2 words
- MESI protocol (Modified, Exclusive, Shared, Invalid)
- Write-back policy

## Directory Structure
```
├── src/
│   ├── cache/              # Direct-mapped cache modules
│   ├── controller/         # MESI controller FSM
│   └── testbench/         # All testbenches
├── docs/                   # Design specs and diagrams
├── sim/                    # Simulation scripts and outputs
└── verification/          # Test cases and coverage
```

## How to Run
[To be added]

## Project Status
- [ ] Direct-mapped cache implementation
- [ ] MESI FSM controller
- [ ] Inter-cache communication
- [ ] Testbench development
- [ ] Verification complete

## References
1. [IEEE Paper 1](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8897321&tag=1)
2. [IEEE Paper 2](https://www.irjet.net/archives/V6/i6/IRJET-V6I6397.pdf)
