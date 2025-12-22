# cpuSimulatorExtended
# Extended CPU Instruction Cycle Simulator

![Von Neumann Architecture](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Von_Neumann_Architecture.svg/800px-Von_Neumann_Architecture.svg.png)

An interactive, single-file HTML/JavaScript simulator demonstrating the classic **fetch → decode → execute** cycle of a simple CPU.

This is an **extended version** of a basic teaching simulator, modified as part of a university group assignment to include advanced instructions, addressing modes, and control flow.

<grok-card data-id="3e91f5" data-type="image_card"></grok-card>



<grok-card data-id="a7088a" data-type="image_card"></grok-card>


## Features (Original + Extensions)

- **Core Cycle**: Step through Fetch, Decode, and Execute phases individually or full instructions.
- **Visual State**: Real-time display of PC, IR, registers (R1–R3), ALU result, zero flag, and memory/program tables.
- **Editable Input**: Write programs and memory directly in textareas.
- **New ALU Instructions**: SUB, MUL, DIV, AND, OR, NOT (with zero flag updates).
- **Immediate Addressing**: `#` prefix (e.g., `LOAD R1, #42`).
- **Register-Indirect**: `(R2)` – address from register.
- **Indexed Addressing**: `500(R2)` – base offset + register value.
- **Conditional Branch**: `JNZ address` – jump if zero flag is false.

<grok-card data-id="32c02f" data-type="image_card"></grok-card>



<grok-card data-id="a406c7" data-type="image_card"></grok-card>



<grok-card data-id="5c15d2" data-type="image_card"></grok-card>


## How to Run

1. Clone or download the repository.
2. Open `cpu_simulator_extended.html` (or the main HTML file) in any modern browser (Chrome, Firefox, Edge).
3. No server needed – runs completely offline!

Edit the program and memory textareas, click **Apply / Reset CPU**, then use **Step Phase** or **Run Until End**.

## Project Structure
├── cpu_simulator_extended.html     # Main simulator (single file with embedded JS/CSS)
├── test1_alu_and_immediate.txt    # Test program 1
├── test2_addressing_modes.txt     # Test program 2
├── test3_jnz_loop.txt             # Test program 3
├── Technical_Report.pdf           # Full report (1000–1500 words)
└── README.md                      # This file
