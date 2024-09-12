### 32-bit 5-Stage Pipelined MIPS Processor

---

#### **Project Overview**

This project implements a 32-bit 5-stage pipelined MIPS processor in Verilog HDL. The processor supports a subset of the MIPS32 instruction set, designed to showcase instruction-level parallelism and improve execution throughput through pipelining.

#### **Table of Contents**

1. [Features](#features)
2. [Getting Started](#getting-started)
   - [System Requirements](#system-requirements)
   - [Installation](#installation)
   - [Setting Up the Environment](#setting-up-the-environment)
3. [Usage](#usage)
   - [Running Simulations](#running-simulations)
   - [Loading Programs](#loading-programs)
   - [Supported Instructions](#supported-instructions)
4. [Programming Guide](#programming-guide)
   - [Assembly Language](#assembly-language)
   - [Example Programs](#example-programs)
5. [Contributing](#contributing)
6. [License](#license)
7. [Contact](#contact)

---

### **Features**

- **5-Stage Pipeline**: Includes Instruction Fetch (IF), Instruction Decode (ID), Execution (EX), Memory Access (MEM), and Write Back (WB) stages.
- **Supported Instructions**: Arithmetic operations, memory access, and branching.
- **Verilog Implementation**: Modular design with separate modules for ALU, control unit, register file, and memory.

---

### **Getting Started**

#### **System Requirements**

- A Verilog-compatible simulator (e.g., ModelSim, VCS).
- FPGA development tools (optional, e.g., Xilinx Vivado, Intel Quartus).
- Knowledge of Verilog HDL and MIPS architecture.

#### **Installation**

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Akor-Michael/MIPS-Processor-32-Bit
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd mips-processor
   ```

#### **Setting Up the Environment**

1. **Install the Simulator**: Ensure you have a Verilog simulator installed on your system.
2. **Open the Project**: Load the Verilog files into your simulator or FPGA development environment.
3. **Compile the Design**: Follow the simulator or FPGA tool instructions to compile the Verilog code.

---

### **Usage**

#### **Running Simulations**

1. **Load the Testbench**: Use the provided testbench to initialize the processor and set up the simulation environment.
2. **Run the Simulation**: Start the simulation and observe the waveforms and outputs.
3. **Check Results**: Verify the results in the register file and memory.

#### **Loading Programs**

1. **Write Assembly Code**: Create your MIPS assembly program.
2. **Assemble the Code**: Convert the assembly code into machine code.
3. **Load into Memory**: Insert the machine code into the processor’s instruction memory.

#### **Supported Instructions**

- **Arithmetic**: `add`, `sub`, `and`, `or`, `slt`
- **Memory Operations**: `lw` (load word), `sw` (store word)
- **Control/Branch**: `beq` (branch on equal), `j` (jump)

---

### **Programming Guide**

#### **Assembly Language**

Write MIPS assembly code using standard syntax:

```asm
addi $t0, $zero, 5
addi $t1, $zero, 10
add $t2, $t0, $t1
```

#### **Example Programs**

- **Simple Addition**:

  ```asm
  addi $t0, $zero, 5
  addi $t1, $zero, 10
  add $t2, $t0, $t1
  ```

- **Memory Load/Store**:

  ```asm
  lw $t0, 0($s0)
  addi $t1, $t0, 1
  sw $t1, 0($s0)
  ```

---

### **Contributing**

If you want to contribute to this project, please follow these guidelines:

1. **Fork the Repository**: Create a personal fork of the repository.
2. **Create a Branch**: Develop your changes in a separate branch.
3. **Submit a Pull Request**: Open a pull request with a detailed description of your changes.

---

### **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

### **Contact**

For questions or feedback, please contact:

- **Author**: Akor Michael
- **Email**: <akormichaeljohn@gmail.com>
- **GitHub**: [yourusername](https://github.com/yourusername)

---

**Happy Assembly Coding!**
