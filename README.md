# RISC-V-SingleCycle-Processor-Design
This repository show the design and implementation of a 3-stage pipelined processor built on the RISC-V Instruction Architecture

# Instructions:

Data Processing: R-type (ADD, SUB, XOR), I-type (ADDI, XORI), U-type (LUI, AUIPC).
Memory Access: I-type (LB, LW), S-type (SW).
CSR & Interrupts: CSRRW, MRET, timer interrupts handled via mip and mepc registers.
Testing & Validation
Validated with GCD and factorial programs

# Compilation & Simulation

Compile using compile.bat or vlog *.sv.
Simulate with vsim -c top_level_module_name -do "run -all".
Use GTKWave to visualize simulation results from the generated processor.vcd dump file:
bash
Copy code
gtkwave processor.vcd
This project demonstrates efficient instruction handling, interrupt management, and hazard resolution, showcasing a robust RISC-V pipelined design.
