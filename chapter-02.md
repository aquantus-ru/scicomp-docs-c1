# CHAPTER 2: Computer Systems Architecture

This chapter explores the physical and logical design of computer systems, bridging the gap between hardware and software.

## 1. The von Neumann Architecture
Proposed by John von Neumann in 1945, this architecture forms the basis of almost all modern computers. Its key characteristics include:
- **Stored-Program Concept**: Instructions and data are stored in the same main memory.
- **Sequential Execution**: Instructions are fetched and executed one after another.
- **Components**:
  - Central Processing Unit (CPU) containing the Control Unit and Arithmetic Logic Unit (ALU).
  - Memory Unit.
  - Input/Output mechanisms.
  - A system bus for data transfer.

The "**von Neumann bottleneck**" refers to the limitation in throughput caused by the shared bus for both data and instructions.

## 2. CPU: Fetch-Decode-Execute Cycle
The **machine cycle** is the operational loop of the CPU:
1. **Fetch**: The CPU retrieves the next instruction from memory address stored in the Program Counter (PC) and loads it into the Instruction Register (IR).
2. **Decode**: The Control Unit interprets the instruction's opcode to determine what action to perform.
3. **Execute**: The CPU performs the operation (e.g., ALU calculation, data movement).
4. **Write-back**: The result is written to a register or memory.

## 3. Memory Hierarchy (Registers, Cache, RAM)
To balance speed, capacity, and cost, memory is organized in a hierarchy:
- **Registers**: Located inside the CPU. Fastest, smallest capacity. Holds immediate operands.
- **Cache (L1, L2, L3)**: SRAM located near the CPU. Stores frequently accessed data (temporal and spatial locality). Faster than RAM but expensive.
- **RAM (Random Access Memory)**: DRAM. Main working memory. Volatile.
- **Secondary Storage**: SSD/HDD. Non-volatile, large capacity, slow.

## 4. Instruction Sets and Assembly
An **Instruction Set Architecture (ISA)** defines the set of operations a processor can execute.
- **CISC (Complex Instruction Set Computer)**: Many specialized instructions (e.g., x86).
- **RISC (Reduced Instruction Set Computer)**: Fewer, simpler instructions (e.g., ARM, MIPS), relying on the compiler to optimize.

**Assembly language** is the human-readable representation of machine code. It uses mnemonics (like `MOV`, `ADD`, `JMP`) instead of raw binary. There is a one-to-one mapping between assembly instructions and machine code.
