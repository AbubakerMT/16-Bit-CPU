# 🛠️ 16-Bit Pipelined Processor Design (MIPS-like CPU)

This project implements a **16-bit pipelined MIPS-like processor** using **Logisim**. The processor features a **single-cycle** and **pipelined architecture**, supporting R-type, I-type, and J-type instructions with **hazard detection and forwarding mechanisms**.

## 🎯 Objectives
- **Design a 16-bit Pipelined Processor** with 8 general-purpose registers.
- **Implement using Logisim** to simulate and test CPU operations.
- **Develop a Single-Cycle Processor** before transitioning to pipelined execution.
- **Ensure pipeline efficiency** by handling hazards and dependencies.
- **Perform extensive simulation** using test cases like Bubble Sort and One Counter.

## 🛠️ Features
- ✨ **General-Purpose Registers:** 8 registers (R0-R7) with R0 hardwired to zero.
- ⚙️ **Instruction Set:** Supports 30 instructions categorized as R-type, I-type, and J-type.
- 📜 **Memory Structure:** 4096-word memory (16-bit per word) with separate instruction and data memory.
- 🔄 **Pipeline Execution:** Implements **hazard detection, forwarding logic, and control unit design**.
- 🎮 **Testing Programs:** Includes Bubble Sort, One Counter, and random test cases.

## 📌 Project Structure
- **PC Control Unit:** Determines memory address fetching and jump/branch execution.
- **Instruction Memory:** Stores and fetches machine code instructions.
- **Register File:** Holds general-purpose registers and manages read/write operations.
- **ALU:** Executes arithmetic and logic computations.
- **Data Memory:** Manages storage and retrieval of data for load/store instructions.
- **Control Signals Unit:** Generates control signals based on opcode and function codes.
- **Pipeline Hazard & Forwarding Logic:** Resolves data dependencies and stalls pipeline when necessary.

## 🎓 Development Process
- **Signal Coordination:** Generated correct control signals for seamless execution.
- **Testing & Debugging:** Used comprehensive test cases to validate the design.
- **Final Integration:** Combined all modules to construct the fully functional processor.

## 🔄 Simulation & Testing
### ✅ **Single-Cycle Processor Tests**
- **Bubble Sort**  
  - Successfully sorted an array using load, store, and branch instructions.
- **One Counter**  
  - Counted the number of '1's in a register value.
- **Random Test Case**  
  - Executed an instructor-provided test case with expected results.

### ✅ **Pipelined Processor Tests**
- **Bubble Sort**  
  - Encountered a stall issue preventing full execution.
- **One Counter**  
  - Produced correct results matching the single-cycle execution.
- **Random Test Case**  
  - Encountered an infinite loop but generated an output close to expectations.

---

## 🖼️ Screenshots

| Description                               | Image                                                      |
|-------------------------------------------|------------------------------------------------------------|
| **Block diagram of the 16-bit processor** | ![Processor Block Diagram](path/to/processor_block_diagram.png) |
| **Simulation of Bubble Sort in Logisim**  | ![Bubble Sort Simulation](path/to/bubble_sort_simulation.png) |
| **Pipelined processor with pipeline stages** | ![Pipelined Processor](path/to/pipelined_processor.png)       |

