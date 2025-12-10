# Implementation of Symmetric Multiprocessing Dual-core system  using MESI Cache Coherence  Protocol
Dual-core cache coherence system implementing the MESI (Modified, Exclusive, Shared, Invalid) protocol in SystemVerilog. This project addresses the fundamental challenge of data consistency in multiprocessor systems. It includes two direct-mapped 512KB caches with 2-word block size, utilizing a write-back policy, and write-invalidate mechanism. This is a project for high-speed multiprocessor system design, specifically maintaining coherency between two processor cores.

## Specifications
The design adheres to the following core parameters:
- **Architecture:** Dual-core Symmetric Multiprocessing (SMP) system.
- **Caches:** 2x 512KB direct-mapped caches
- **Block size:** 2 words
- **Protocol:** MESI protocol (Modified, Exclusive, Shared, Invalid)
- **Write Policy:** Write-back with Write-invalidate mechanism. When a processor writes to a shared location, all copies in other caches are invalidated.
- **Implementation Language:** SystemVerilog.

## Directory Structure
```
This structure reflects the modular design of the SystemVerilog implementation:
├── src/
│   ├── req_buffer/        # Request buffer module (for handling pending bus requests)
│   ├── cache/             # Direct-mapped cache modules (Data array, tag array, state bits)
│   ├── controller/        # MESI controller FSM (Handles core requests and snoop events)
│   └── testbench/         # All SystemVerilog testbenches and stimulus
├── docs/                  # Detailed design document, block diagrams, and interface definitions
├── sim/                   # Simulation scripts and outputs (e.g., waves/logs)
└── verification/          # Verification plan, specific test cases, and coverage reports
```

## License
This project is licensed under the MIT License - see the LICENSE.txt file for details. 

## References
1. [IEEE Paper 1](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8897321&tag=1)
2. [IEEE Paper 2](https://www.irjet.net/archives/V6/i6/IRJET-V6I6397.pdf)
