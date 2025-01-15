# Digital Logic Circuits and Computer Architecture - Class Notes

## UNIT I: Introduction to Digital Logic Circuits

### 1. Introduction to Digital Logic Circuits
- **Definition:** Digital circuits process binary data (0 and 1).
- **Logic Gates:** Basic building blocks (AND, OR, NOT).
- **Use:** Foundational in computers and digital devices.

### 2. Number System
- **Binary (Base 2):** Uses 0 and 1.
- **Decimal (Base 10):** Uses 0 to 9.
- **Conversion:**
  - Decimal to Binary: Divide by 2, record remainders.
  - Binary to Decimal: Multiply each bit by 2 raised to its position index.

### 3. Complements
- **1's Complement:** Invert all bits.
- **2's Complement:** Add 1 to the 1's complement.
- **Usage:** Simplifies binary subtraction.

### 4. Binary Codes
- **BCD (Binary Coded Decimal):** Represents decimal numbers in binary form (4 bits per digit).
- **Gray Code:** Binary code where two successive values differ in only one bit.
- **ASCII:** Standard code for text representation.

### 5. Error Detection Codes
- **Parity Bits:** Add a bit to make the number of 1s either even (even parity) or odd (odd parity).
- **Hamming Code:** Error correction code that can detect and correct single-bit errors.

### 6. Logic Gates
- **AND Gate:** Output is 1 if both inputs are 1.
- **OR Gate:** Output is 1 if at least one input is 1.
- **NOT Gate:** Inverts the input.
- **Truth Tables:** Used to define the function of a gate.

### 7. Boolean Algebra
- **Operations:** AND (.), OR (+), NOT (')
- **Laws:**
  - Identity: A + 0 = A, A . 1 = A
  - Null: A + 1 = 1, A . 0 = 0
  - Idempotent: A + A = A, A . A = A
  - Complement: A + A' = 1, A . A' = 0

### 8. Maps Simplification (Karnaugh Maps)
- **K-map:** A grid used to simplify Boolean expressions.
- **Grouping:** Combine adjacent 1s in groups of 1, 2, 4, etc.
- **Simplification:** Reduces the number of terms in a Boolean expression.

---

## UNIT II: Basic Structure of Computers and Data Representation

### 9. Basic Structure of Computers: Computer Types
- **Types:** Microcomputers, Minicomputers, Mainframes, Supercomputers.
- **Usage:** Varies based on size and performance needs.

### 10. Functional Unit
- **Components:**
  - ALU (Arithmetic Logic Unit): Performs arithmetic and logical operations.
  - CU (Control Unit): Directs operations of the processor.
  - Memory: Stores data and instructions.
  - I/O Devices: Input and output data.

### 11. Basic Operational Concepts
- **Fetch-Decode-Execute Cycle:**
  1. Fetch instruction from memory.
  2. Decode the instruction.
  3. Execute the instruction.

### 12. Bus Structures
- **Types:** Data bus, Address bus, Control bus.
- **Function:** Transfers data between components.

### 13. Data Representation: Fixed Point and Floating-Point Representation
- **Fixed Point:** Represents integers.
- **Floating Point:** Represents real numbers, using a mantissa and exponent.
- **Standard:** IEEE 754 for floating-point representation.

### 14. Register Transfer Language (RTL)
- **RTL:** Describes operations in terms of data transfers between registers.
- **Example:** R1 <- R2 means data in R2 is transferred to R1.

### 15. Register Transfer, Bus, and Memory Transfers
- **Memory Read:** Transfer data from memory to a register.
- **Memory Write:** Transfer data from a register to memory.

---

## UNIT III: Pipeline and Vector Processing & Multiprocessors

### 16. Pipeline and Vector Processing: Parallel Processing
- **Parallel Processing:** Multiple processors execute tasks simultaneously.
- **SIMD:** Single Instruction, Multiple Data.

### 17. Pipelining
- **Stages:**
  1. Instruction Fetch
  2. Instruction Decode
  3. Execute
  4. Memory Access
  5. Write Back
- **Hazards:** Data, Control, Structural.

### 18. Arithmetic Pipeline
- **Usage:** Pipelines in arithmetic operations like addition and multiplication.
- **Stages:** Divides the task into subtasks, executed in pipeline stages.

### 19. Instruction Pipeline
- **Description:** Overlaps execution of instructions to increase throughput.
- **Example:** Fetch next instruction while current one is being decoded.

### 20. Characteristics of Multiprocessors
- **Symmetric Multiprocessing (SMP):** All processors share memory equally.
- **Asymmetric Multiprocessing (AMP):** Specific roles for processors.

### 21. Interconnection Structures (various types)
- **Types:** Bus, Crossbar, Multistage networks.
- **Purpose:** Connects processors, memory, and I/O devices.

---

## UNIT IV: Architecture of Microprocessors and Assembly Language

### 22. Introduction to Microprocessors
- **Definition:** A CPU on a single chip.
- **Evolution:** From simple 4-bit processors to complex multicore CPUs.

### 23. Overview of 8086 Microprocessor
- **Architecture:** 16-bit processor, segmented memory.
- **Registers:** General purpose, segment, pointer, index.

### 24. Signals and Pins of 8086
- **Important Pins:**
  - AD0-AD15: Address/Data lines.
  - ALE: Address Latch Enable.
  - RD, WR: Read/Write control signals.

### 25. Physical Memory Organization
- **Segmentation:** Divides memory into segments for efficient management.
- **Segments:** Code, Data, Stack, Extra.

### 26. Assembly Language of 8086 (various topics)
- **Instructions:**
  - MOV: Transfer data.
  - ADD: Add data.
  - JMP: Jump to another instruction.

### 27. Assembler Directives and Operators
- **Directives:** Instructions for the assembler, like ORG, END.
- **Operators:** Used in expressions, like +, -, *, /.

### 28. Assembly Software Programs with Algorithms
- **Example:**
  - Factorial Calculation.
  - Greatest Common Divisor (GCD).

---

## UNIT V: Interfacing with 8086

### 29. Interfacing with RAMs, ROMs, Peripheral ICs
- **Purpose:** Allows 8086 to communicate with memory and peripherals.
- **Address Decoding:** Ensures correct selection of memory or device.

### 30. ADCs and DACs Interfacing
- **ADC:** Converts analog signals to digital.
- **DAC:** Converts digital signals to analog.

### 31. Serial Data Transfer Schemes
- **Synchronous vs. Asynchronous:** Synchronous uses a clock signal, asynchronous does not.
- **UART:** Universal Asynchronous Receiver/Transmitter for serial communication.

### 32. USART 8251 Serial Data Communication
- **Modes:** Synchronous and Asynchronous communication.
- **Initialization:** Setting baud rate, data bits, stop bits, parity.

### 33. Interrupt Vector Table
- **IVT:** Holds addresses of interrupt service routines.
- **Structure:** Fixed locations for different interrupts.

### 34. Interrupt Structure with 8259
- **8259 PIC:** Manages hardware interrupts.
- **Priority:** Determines the order in which interrupts are handled.

---

## Study Schedule

### Week 1
- Topics 1-8

### Week 2
- Topics 9-15

### Week 3
- Topics 16-21

### Week 4
- Topics 22-28

### Week 5
- Topics 29-34

---

## Exam Preparation Tips
- Understand concepts rather than memorizing.
- Solve practice problems.
- Use diagrams for visualization.

---

These class notes offer a summary of each topic for quick review and reference during your study sessions.
