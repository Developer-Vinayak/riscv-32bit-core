# Stage 1: Encoding & Decoding (RISC-V)

This document outlines the manual encoding and decoding process for 32-bit RISC-V instructions.

## 1. Encoding: 32-bit Instruction for `add x3, x1, x2`

**Instruction:** `add x3, x1, x2`
**Type:** R-Type

### Bit Breakdown

| Field | Funct7 | rs2 | rs1 | funct3 | rd | opcode |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Value** | 0000000 | 00010 | 00001 | 000 | 00011 | 0110011 |
| **Bits** | 31-25 | 24-20 | 19-15 | 14-12 | 11-7 | 6-0 |

*Note: `x3=3`, `x1=1`, `x2=2`*

### Hexadecimal Result
`0x002081B3`

---

## 2. Decoding: Hex to Instruction

**Hex Input:** `0x003100B3`

### Step 1: Binary Conversion
```text
0000 0000 0011 0001 0000 0000 1011 0011
