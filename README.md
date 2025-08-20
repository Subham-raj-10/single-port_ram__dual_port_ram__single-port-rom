## 📘 Memory Modules in Verilog

This repository contains Verilog HDL implementations of fundamental memory architectures, including:
🟦 Single-Port RAM (64 x 8-bit)
🟪 Dual-Port RAM (64 x 8-bit)
🟨 Single-Port ROM (16 x 4-bit example)
Each module is synthesizable and verified through testbenches and simulation waveforms.
These designs form the building blocks of digital systems, processors, and FPGA applications.


## 1. Single-Port RAM (64 x 8-bit)
A Single-Port RAM allows both read and write operations using a single address/data interface.

*Features :*
64 memory locations, each 8 bits wide.
Single address bus and data bus.
Controlled by clk and we (write_enable) signals.



 ## 2. Dual-Port RAM (64 x 8-bit)
A Dual-Port RAM supports simultaneous memory access from two independent ports (A & B).


*Features:*
64 memory locations, 8-bit wide.
Independent read/write ports (A and B).
Separate address and write-enable per port.
Allows concurrent operations.



## 3. Single-Port ROM (16 x 4-bit)
A Read-Only Memory (ROM) is preloaded with fixed values and supports only read operations.

*Features:*
16 memory locations, each 4 bits wide (example configuration).
Lookup-table style access.
Used for constants, microcode, and fixed storage.

## ⚙️ Tools & Setup
HDL: Verilog
Verification: Testbenches with waveform analysis.

## 🚀 Applications
Cache memory & buffer design.
Lookup tables for DSP and AI accelerators.
Microcode storage in processors.
Multi-core & parallel memory systems (using dual-port RAM).
