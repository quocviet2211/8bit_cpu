

## 1. Project Overview
<img width="1207" height="639" alt="image" src="https://github.com/user-attachments/assets/d558d24c-243e-4eba-920e-4d01f4960300" />
# 4-Bit RISC CPU Design Using Verilog
This project implements a 4-bit RISC CPU using Verilog HDL. The processor uses a 3-stage pipeline:

- IF (Instruction Fetch)
- ID (Instruction Decode)
- EX (Execute)

The design includes a program counter, instruction memory, control unit, register file, ALU, data memory, pipeline registers, and status flags.

## 2. Architecture

The CPU follows a modular design. The program counter selects the instruction address, instruction memory provides the instruction, the control unit decodes it, and the ALU performs the required operation.

The pipeline allows different instructions to occupy different processing stages during the same clock cycle.

## 3. Main Components

- Program Counter (PC)
- Instruction Memory
- Instruction Decoder
- Control Unit
- Register File
- Arithmetic Logic Unit (ALU)
- Data Memory
- Pipeline Registers
- Flag Register
- Branch and Jump Control

## 4. Project Structure

- `src/`: CPU modules written in Verilog
- `testbench/`: CPU verification testbench
- `programs/`: Memory initialization files
- `docs/`: Architecture diagrams and simulation results

## 5. Verification

The CPU is tested with several programs:

- `program.mem`: Demonstration program
- `prog_arith.mem`: Arithmetic operations
- `prog_logic.mem`: Logic operations
- `prog_jump.mem`: Jump instructions

The testbench checks instruction execution, register values, program counter behavior, and pipeline operation.

## 6. Tools

- Verilog HDL
- Xilinx Vivado
- Behavioral Simulation

