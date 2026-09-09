# Stheffanny N. Alves

**Computer Engineering undergraduate — Embedded Systems, Firmware & Embedded Security**

I'm an undergraduate in Computer Engineering at UEFS. My focus is low-level software: bare-metal firmware, ARM Cortex-M0+, debug protocols (SWD), and firmware security. I build toward embedded security research as a long-term goal, and work in Java/Spring Boot backend as a parallel, more immediately employable track — the two feed into the same longer-term interest: backend systems that orchestrate hardware fleets (IoT/Edge).

I'm a member of the IEEE Robotics and Automation Society (RAS) and Women in Engineering (WIE) chapters at UEFS.

## Featured project

**[Dolos — SWD Forensic Extractor](https://github.com/StheffannyNAlves/swd-forensic-extractor)**

A bare-metal firmware acquisition tool: one RP2040 (Pico H) acts as a forensic SWD probe against a second RP2040, written in ARM Cortex-M0+ assembly with a multicore split (Core 1 dedicated to the SWD bit-bang timing, Core 0 for USB CDC/logging).

Current status: Phase 2 — IDCODE handshake validation, working through an ACK=7 response on the target (currently isolating whether it's a protocol timing issue or a physical wiring fault). Architecture and design decisions — forensic QSPI init rationale, LUT-based error policy, planned v2 offensive mode (payload injection via DCRSR/DCRDR, FPB breakpoints) — are documented in an internal spec, currently at Rev. 5.

`C` · `ARM Assembly` · `RP2040` · `SWD` · `USB` · `CMake` · `Python`

## Other work

**[RP2040 Bare-Metal Research](https://github.com/StheffannyNAlves/Uart-baremetal-rp2040)**
Boot process, runtime init, memory layout and peripheral access on RP2040 without the Pico SDK.
`C` · `ARM Assembly` · `RP2040` · `MMIO` · `UART` · `Linker Script`

**[Data Structures & Graph Algorithms](https://github.com/StheffannyNAlves/estrutura-de-dados)**
Core data structures in C (linked list, stack, queue, AVL, B-tree, hash tables with chaining and linear probing) and graph algorithms in C++ (DFS, Kahn's topological sort, Kruskal's MST with Union-Find, Prim's MST).
`C` · `C++`

**[Forkeazando](https://github.com/StheffannyNAlves/Forkeazando)**
Interactive narrative game (visual novel) satirizing the trajectory through a Computer Engineering degree, built in Java with a two-person team as a PBL course project. Includes a branching-chapter structure driven by accumulated in-game score/participation, and a class model deliberately built without inheritance between protagonist and secondary characters — a justified design decision, not a default.
`Java` · `Maven`

## Currently exploring

Secure boot, fault injection, reverse engineering.

## Academic

B.Sc. in Computer Engineering (in progress) — Universidade Estadual de Feira de Santana (UEFS)

## Languages

![Top languages](https://github-readme-stats.vercel.app/api/top-langs?username=StheffannyNAlves&layout=compact&langs_count=8)

## Contact

- GitHub: [StheffannyNAlves](https://github.com/StheffannyNAlves)
- LinkedIn: [Stheffanny Nascimento](https://linkedin.com/in/stheffannynascimento)
