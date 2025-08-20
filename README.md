## 📘 Memory Modules in Verilog
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
This repository contains Verilog HDL implementations of fundamental memory architectures, including:
🟦 Single-Port RAM (64 x 8-bit)
🟪 Dual-Port RAM (64 x 8-bit)
🟨 Single-Port ROM (16 x 4-bit example)
Each module is synthesizable and verified through testbenches and simulation waveforms.
These designs form the building blocks of digital systems, processors, and FPGA applications.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 1. Single-Port RAM (64 x 8-bit)
A Single-Port RAM allows both read and write operations using a single address/data interface.

*Block Diagram*
<img width="841" height="916" alt="single_port_blockdiagram_64-8" src="https://github.com/user-attachments/assets/d0f95ee9-7b99-48c3-9b9b-5d13051e76da" />

*Features :*
64 memory locations, each 8 bits wide.
Single address bus and data bus.
Controlled by clk and we (write_enable) signals.

*Simulation:*
<img width="1555" height="278" alt="single_port_ram_op" src="https://github.com/user-attachments/assets/59578953-ecf1-4b56-8f93-33f630b8401b" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 ## 2. Dual-Port RAM (64 x 8-bit)
A Dual-Port RAM supports simultaneous memory access from two independent ports (A & B).

*Block Diagram*
<img width="537" height="633" alt="dual_port_ram_64-8" src="https://github.com/user-attachments/assets/7a93b6c1-dc3a-4d59-996a-8a44d50c246c" />

*Features:*
64 memory locations, 8-bit wide.
Independent read/write ports (A and B).
Separate address and write-enable per port.
Allows concurrent operations.

*Simulation:*
<img width="1577" height="437" alt="dual_port_ram_tb" src="https://github.com/user-attachments/assets/06c3e544-cdda-42a2-a05b-959d166bec5a" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 3. Single-Port ROM (16 x 4-bit)
A Read-Only Memory (ROM) is preloaded with fixed values and supports only read operations.

*Features:*
16 memory locations, each 4 bits wide (example configuration).
Lookup-table style access.
Used for constants, microcode, and fixed storage.

*Simulation:*
<img width="1572" height="338" alt="rom_output" src="https://github.com/user-attachments/assets/0a874f5d-fec0-458e-81ec-d1af1d4419ab" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## ⚙️ Tools & Setup
HDL: Verilog
Verification: Testbenches with waveform analysis.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 🚀 Applications
Cache memory & buffer design.
Lookup tables for DSP and AI accelerators.
Microcode storage in processors.
Multi-core & parallel memory systems (using dual-port RAM).
