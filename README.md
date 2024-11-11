# 8-Bit-Modified-SAP-Design
Assignment: 8-Bit Modified SAP (Simple-As-Possible) Design

Introduction
The primary objective of this assignment is to design an 8-bit microinstruction sequencer that generates control words to execute specific instructions. Using ISIS software, we validated the generated control words by simulating them for the given instructions.

1. Block Diagram of MSAP
The MSAP (Modified Simple-As-Possible) design includes a microinstruction sequencer, a control word generator, and associated control blocks.
2. Control Word Design in Binary Format
The control word for MSAP is designed by enabling relevant pins across different MSAP blocks, translating instructions into binary format. For efficient storage, we convert the 32-bit control word to an 8-bit hexadecimal file compatible with the ROM memory format. This conversion allows four ROMs to be connected in sequence, each storing a part of the control word.

Using MATLAB, we then convert these hexadecimal values to binary (or machine) files, which are loaded into the ROM block to configure the MSAP.

Figure: The 8-bit Hexadecimal Control Word Design Diagram (note: illustration should show how binary data is stored and represented in ROM).

3. Working Procedure
Reset the memory block.
Load data into RAM.
Input data using a keyboard interface.
Activate the ready pin to initiate input reading.
These steps prepare the system for processing and executing instructions based on the control word sequence.
4. Instruction Execution and Output
Opcode Table:
The system processes each opcode with instructions like IN A, INC B, MOV, RCL, XOR, and OUT.
The control word manipulates registers A, B, C, and D to reflect instruction effects.
Example:

Opcode: 00 - Instruction: IN A - Registers: A = 13, B = 00, C = 00, D = 00
Opcode: 06 - Instruction: XOR A, B - Result: A = F0, B = 18, C = 0A, D = 18
Conclusion
The 8-bit modified SAP design is a simplified yet functional approach to understanding fundamental computing operations in microprocessors.
