# Comprehensive Topic Questions

## Architecture Fundamentals
1. Compare and contrast computer architecture and computer organization. How do they differ in terms of their focus and concerns?

2. Explain the relationship between Instruction Set Architecture (ISA) and computer architecture. Why is ISA significant?

3. How does the concept of backwards compatibility relate to computer architecture? Use the Intel x86 family as an example.

## Computer Structure and Function
1. What are the four basic functions that a computer can perform? Explain each one and how they interact.

2. Draw and explain the structure of a simple single-processor computer. What are its main components?

3. In terms of structure and function, how does the Control Unit relate to the overall operation of the CPU?

## Modern Computer Organization
1. Compare and contrast the structure of a single-core processor with a multicore processor. What are the key differences?

2. Analyze the role of different cache levels (L1, L2, L3) in a modern processor. How do they improve performance?

3. Using the IBM z13 as an example, explain the purpose of different functional units within a processor core.

# Flashcard Questions

## Basic Concepts
Q: What is computer architecture?
A: The attributes of a system visible to a programmer that have a direct impact on the logical execution of a program.

Q: What are the four main structural components of a CPU?
A: 1) Control Unit 2) Arithmetic Logic Unit 3) Registers 4) CPU Interconnection

Q: What is the difference between a processor and a core?
A: A processor is a physical piece of silicon that can contain one or more cores, while a core is an individual processing unit on a processor chip.

## Hardware Components
Q: What is a motherboard?
A: The main printed circuit board in a computer that holds and allows communication between crucial electronic components like the CPU and memory.

Q: What are the three main types of cache typically found in modern processors?
A: L1 Cache (split into instruction and data), L2 Cache, and L3 Cache

Q: What is the primary function of the Load/Store logic in a CPU core?
A: It manages the transfer of data to and from main memory via cache.

## Advanced Concepts
Q: What is ISU (Instruction Sequence Unit) responsible for?
A: It determines instruction execution sequence in superscalar architecture, enables out-of-order pipeline, and tracks register names and instruction dependencies.

Q: What are the four basic functions of a computer system?
A: 1) Data Processing 2) Data Storage 3) Data Movement 4) Control

Q: What is the purpose of the Recovery Unit (RU) in the IBM z13 core?
A: It keeps a copy of the complete system state, collects hardware fault signals, and manages hardware recovery actions.

## Design and Implementation
Q: What is an organizational design issue in computer architecture?
A: How specific features are implemented, such as whether a multiply instruction uses a dedicated multiply unit or repeated addition.

Q: What is the primary purpose of the system bus?
A: To provide communication among CPU, Main Memory, and I/O components through a set of conducting wires.

Q: What is the role of the LSU (Load-Store Unit)?
A: It contains the L1 data cache and manages data traffic between the L2 data cache and functional execution units.