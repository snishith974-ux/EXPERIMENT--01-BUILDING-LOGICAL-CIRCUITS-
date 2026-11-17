# EXPERIMENT-01: BUILDING LOGICAL CIRCUITS

## NAME:
## ROLL NUMBER:RA2511030010327
## DEPARTMENT:NWC



## 1. Aim

To design, implement, simplify, and verify combinational logic circuits using Boolean algebra and digital logic gates.

## 2. Boolean Notation

Use the following notation throughout this experiment:

| Symbol | Meaning | Example |
|---|---|---|
| `!A` | NOT A | `!A` |
| `A & B` | AND | `A & B` |
| `A \| B` | OR | `A \| B` |
| `A ^ B` | XOR | `A ^ B` |
| `A XNOR B` | XNOR | `A XNOR B` |

**Important:** In these equations, `!` means NOT, `&` means AND, `|` means OR, and `^` means XOR. Parentheses determine the order of operations.

## 3. Advanced Boolean Equations

### Equation 1: Four-Input Sum-of-Products

```text
F1 = (!A & B & C)
   | (A & B & !D)
   | (!B & C & D)
   | (A & !C & D)
```

**Inputs:** A, B, C, D  
**Output:** F1  
**Challenge:** Simplify the expression and compare gate counts.

### Equation 2: Product-of-Sums Circuit

```text
F2 = (A | !B | C)
   & (!A | B | D)
   & (B | !C | !D)
```

**Inputs:** A, B, C, D  
**Output:** F2  
**Challenge:** Implement the circuit using NAND gates and verify functional equivalence.

### Equation 3: Nested Complement Logic

```text
F3 = !(
       ((! (A | B)) | (C & D))
       &
       (A | (!(B | C)))
     )
```

**Inputs:** A, B, C, D  
**Output:** F3  
**Challenge:** Apply De Morgan's theorems and implement the circuit using NAND and NOR gates.

### Equation 4: XOR-XNOR Combinational Circuit

```text
F4 = ((A XOR B) & (C XNOR D))
   | (!A & B & (C XOR D))
```

**Inputs:** A, B, C, D  
**Output:** F4  
**Challenge:** Compare an XOR/XNOR implementation with a basic-gate implementation.

### Equation 5: Five-Input Logic Function

```text
F5 = (A & B & !C)
   | (!A & D & E)
   | (B & C & !E)
   | (!B & C & D)
```

**Inputs:** A, B, C, D, E  
**Output:** F5  
**Challenge:** Generate and verify all 32 input combinations.

### Equation 6: Six-Input Mixed Logic

```text
F6 = ((A | B) & !(C | D))
   | ((C XOR E) & (D | G))
   | (!A & B & E)
```

**Inputs:** A, B, C, D, E, G  
**Output:** F6  
**Challenge:** Calculate gate count and logic depth. Verify all 64 input combinations.

### Equation 7: NAND-NOR Hybrid Logic

```text
F7 = (! (A & B) & !(C | D))
   | (!(A | C) & B & D)
```

**Inputs:** A, B, C, D  
**Output:** F7  
**Challenge:** Implement the function using NAND and NOR gates with any required input inversions.

### Equation 8: Six-Input Advanced Combinational Logic

```text
F8 = ((A XOR B) & (C XNOR D))
   | (!(A | B) & C & E)
   | (A & B & !(D | F))
```

**Inputs:** A, B, C, D, E, F  
**Output:** F8  
**Challenge:** Simplify the expression, design the circuit, and verify all 64 input combinations.

## 4. Experimental Procedure

1. Identify all input variables and the output.
2. Draw the logic circuit for each equation.
3. Implement the circuit in Logisim Evolution, Proteus, or a digital logic trainer kit.
4. Apply all possible input combinations.
5. Record the expected and observed outputs.
6. Simplify the Boolean expression using Boolean algebra.
7. Build the simplified circuit and compare gate counts.
8. Save the circuit diagrams, truth tables, and verification screenshots.

## 5. Truth Table Requirements

| Number of inputs | Required combinations |
|---:|---:|
| 4 | 16 |
| 5 | 32 |
| 6 | 64 |

Use this format to record the results:

| Inputs | Expected output | Observed output | Status |
|---|---|---|---|
| 0000 |  |  |  |
| 0001 |  |  |  |
| 0010 |  |  |  |
| ... |  |  |  |

Extend the table to include every input combination required by each equation.

For F1 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 0 | 0 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 0 | 0 | PASS |
| 0011 | 1 | 1 | PASS |
| 0100 | 0 | 0 | PASS |
| 0101 | 0 | 0 | PASS |
| 0110 | 1 | 1 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 0 | 0 | PASS |
| 1001 | 1 | 1 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 1 | 1 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 1 | 1 | PASS |
| 1110 | 1 | 1 | PASS |
| 1111 | 0 | 0 | PASS |

For F2 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 1 | 1 | PASS |
| 0001 | 1 | 1 | PASS |
| 0010 | 1 | 1 | PASS |
| 0011 | 0 | 0 | PASS |
| 0100 | 0 | 0 | PASS |
| 0101 | 0 | 0 | PASS |
| 0110 | 1 | 1 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 0 | 0 | PASS |
| 1001 | 1 | 1 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 1 | 1 | PASS |
| 1110 | 1 | 1 | PASS |
| 1111 | 1 | 1 | PASS |

For F3 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 0 | 0 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 1 | 1 | PASS |
| 0011 | 1 | 1 | PASS |
| 0100 | 1 | 1 | PASS |
| 0101 | 1 | 1 | PASS |
| 0110 | 1 | 1 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 1 | 1 | PASS |
| 1001 | 1 | 1 | PASS |
| 1010 | 1 | 1 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 1 | 1 | PASS |
| 1110 | 1 | 1 | PASS |
| 1111 | 0 | 0 | PASS |

For F4 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 1 | 1 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 0 | 0 | PASS |
| 0011 | 1 | 1 | PASS |
| 0100 | 1 | 1 | PASS |
| 0101 | 0 | 0 | PASS |
| 0110 | 0 | 0 | PASS |
| 0111 | 1 | 1 | PASS |
| 1000 | 0 | 0 | PASS |
| 1001 | 0 | 0 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 1 | 1 | PASS |
| 1101 | 0 | 0 | PASS |
| 1110 | 0 | 0 | PASS |
| 1111 | 1 | 1 | PASS |

For F5 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 00000 | 0 | 0 | PASS |
| 00001 | 0 | 0 | PASS |
| 00010 | 0 | 0 | PASS |
| 00011 | 1 | 1 | PASS |
| 00100 | 0 | 0 | PASS |
| 00101 | 0 | 0 | PASS |
| 00110 | 1 | 1 | PASS |
| 00111 | 1 | 1 | PASS |
| 01000 | 0 | 0 | PASS |
| 01001 | 0 | 0 | PASS |
| 01010 | 0 | 0 | PASS |
| 01011 | 1 | 1 | PASS |
| 01100 | 1 | 1 | PASS |
| 01101 | 0 | 0 | PASS |
| 01110 | 1 | 1 | PASS |
| 01111 | 1 | 1 | PASS |
| 10000 | 0 | 0 | PASS |
| 10001 | 0 | 0 | PASS |
| 10010 | 0 | 0 | PASS |
| 10011 | 0 | 0 | PASS |
| 10100 | 0 | 0 | PASS |
| 10101 | 0 | 0 | PASS |
| 10110 | 1 | 1 | PASS |
| 10111 | 1 | 1 | PASS |
| 11000 | 1 | 1 | PASS |
| 11001 | 1 | 1 | PASS |
| 11010 | 1 | 1 | PASS |
| 11011 | 1 | 1 | PASS |
| 11100 | 1 | 1 | PASS |
| 11101 | 0 | 0 | PASS |
| 11110 | 1 | 1 | PASS |
| 11111 | 0 | 0 | PASS |

For F6 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 000000 | 0 | 0 | PASS |
| 000001 | 0 | 0 | PASS |
| 000010 | 0 | 0 | PASS |
| 000011 | 1 | 1 | PASS |
| 000100 | 0 | 0 | PASS |
| 000101 | 0 | 0 | PASS |
| 000110 | 1 | 1 | PASS |
| 000111 | 1 | 1 | PASS |
| 001000 | 0 | 0 | PASS |
| 001001 | 1 | 1 | PASS |
| 001010 | 0 | 0 | PASS |
| 001011 | 0 | 0 | PASS |
| 001100 | 1 | 1 | PASS |
| 001101 | 1 | 1 | PASS |
| 001110 | 0 | 0 | PASS |
| 001111 | 0 | 0 | PASS |
| 010000 | 1 | 1 | PASS |
| 010001 | 1 | 1 | PASS |
| 010010 | 1 | 1 | PASS |
| 010011 | 1 | 1 | PASS |
| 010100 | 0 | 0 | PASS |
| 010101 | 0 | 0 | PASS |
| 010110 | 1 | 1 | PASS |
| 010111 | 1 | 1 | PASS |
| 011000 | 0 | 0 | PASS |
| 011001 | 1 | 1 | PASS |
| 011010 | 1 | 1 | PASS |
| 011011 | 1 | 1 | PASS |
| 011100 | 1 | 1 | PASS |
| 011101 | 1 | 1 | PASS |
| 011110 | 1 | 1 | PASS |
| 011111 | 1 | 1 | PASS |
| 100000 | 1 | 1 | PASS |
| 100001 | 1 | 1 | PASS |
| 100010 | 1 | 1 | PASS |
| 100011 | 1 | 1 | PASS |
| 100100 | 0 | 0 | PASS |
| 100101 | 0 | 0 | PASS |
| 100110 | 1 | 1 | PASS |
| 100111 | 1 | 1 | PASS |
| 101000 | 0 | 0 | PASS |
| 101001 | 1 | 1 | PASS |
| 101010 | 0 | 0 | PASS |
| 101011 | 0 | 0 | PASS |
| 101100 | 1 | 1 | PASS |
| 101101 | 1 | 1 | PASS |
| 101110 | 0 | 0 | PASS |
| 101111 | 0 | 0 | PASS |
| 110000 | 1 | 1 | PASS |
| 110001 | 1 | 1 | PASS |
| 110010 | 1 | 1 | PASS |
| 110011 | 1 | 1 | PASS |
| 110100 | 0 | 0 | PASS |
| 110101 | 0 | 0 | PASS |
| 110110 | 1 | 1 | PASS |
| 110111 | 1 | 1 | PASS |
| 111000 | 0 | 0 | PASS |
| 111001 | 1 | 1 | PASS |
| 111010 | 0 | 0 | PASS |
| 111011 | 0 | 0 | PASS |
| 111100 | 1 | 1 | PASS |
| 111101 | 1 | 1 | PASS |
| 111110 | 0 | 0 | PASS |
| 111111 | 0 | 0 | PASS |

For F7 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 0000 | 1 | 1 | PASS |
| 0001 | 0 | 0 | PASS |
| 0010 | 0 | 0 | PASS |
| 0011 | 0 | 0 | PASS |
| 0100 | 1 | 1 | PASS |
| 0101 | 1 | 1 | PASS |
| 0110 | 0 | 0 | PASS |
| 0111 | 0 | 0 | PASS |
| 1000 | 1 | 1 | PASS |
| 1001 | 0 | 0 | PASS |
| 1010 | 0 | 0 | PASS |
| 1011 | 0 | 0 | PASS |
| 1100 | 0 | 0 | PASS |
| 1101 | 0 | 0 | PASS |
| 1110 | 0 | 0 | PASS |
| 1111 | 0 | 0 | PASS |

For F8 OUTPUT
| Inputs | Expected output | Observed output | Status |
| :---: | :---: | :---: | :---: |
| 000000 | 0 | 0 | PASS |
| 000001 | 0 | 0 | PASS |
| 000010 | 0 | 0 | PASS |
| 000011 | 0 | 0 | PASS |
| 000100 | 0 | 0 | PASS |
| 000101 | 0 | 0 | PASS |
| 000110 | 0 | 0 | PASS |
| 000111 | 0 | 0 | PASS |
| 001000 | 0 | 0 | PASS |
| 001001 | 0 | 0 | PASS |
| 001010 | 1 | 1 | PASS |
| 001011 | 1 | 1 | PASS |
| 001100 | 0 | 0 | PASS |
| 001101 | 0 | 0 | PASS |
| 001110 | 1 | 1 | PASS |
| 001111 | 1 | 1 | PASS |
| 010000 | 1 | 1 | PASS |
| 010001 | 1 | 1 | PASS |
| 010010 | 1 | 1 | PASS |
| 010011 | 1 | 1 | PASS |
| 010100 | 0 | 0 | PASS |
| 010101 | 0 | 0 | PASS |
| 010110 | 0 | 0 | PASS |
| 010111 | 0 | 0 | PASS |
| 011000 | 0 | 0 | PASS |
| 011001 | 0 | 0 | PASS |
| 011010 | 0 | 0 | PASS |
| 011011 | 0 | 0 | PASS |
| 011100 | 1 | 1 | PASS |
| 011101 | 1 | 1 | PASS |
| 011110 | 1 | 1 | PASS |
| 011111 | 1 | 1 | PASS |
| 100000 | 1 | 1 | PASS |
| 100001 | 1 | 1 | PASS |
| 100010 | 1 | 1 | PASS |
| 100011 | 1 | 1 | PASS |
| 100100 | 0 | 0 | PASS |
| 100101 | 0 | 0 | PASS |
| 100110 | 0 | 0 | PASS |
| 100111 | 0 | 0 | PASS |
| 101000 | 0 | 0 | PASS |
| 101001 | 0 | 0 | PASS |
| 101010 | 0 | 0 | PASS |
| 101011 | 0 | 0 | PASS |
| 101100 | 1 | 1 | PASS |
| 101101 | 1 | 1 | PASS |
| 101110 | 1 | 1 | PASS |
| 101111 | 1 | 1 | PASS |
| 110000 | 1 | 1 | PASS |
| 110001 | 0 | 0 | PASS |
| 110010 | 1 | 1 | PASS |
| 110011 | 0 | 0 | PASS |
| 110100 | 0 | 0 | PASS |
| 110101 | 0 | 0 | PASS |
| 110110 | 0 | 0 | PASS |
| 110111 | 0 | 0 | PASS |
| 111000 | 1 | 1 | PASS |
| 111001 | 0 | 0 | PASS |
| 111010 | 1 | 1 | PASS |
| 111011 | 0 | 0 | PASS |
| 111100 | 0 | 0 | PASS |
| 111101 | 0 | 0 | PASS |
| 111110 | 0 | 0 | PASS |
| 111111 | 0 | 0 | PASS |


## 6. Performance Analysis

For each circuit, record:

- Number of AND gates
- Number of OR gates
- Number of NOT gates
- Number of XOR/XNOR gates
- Total gate count
- Logic depth
- Functional equivalence before and after simplification

## 7. Expected Results

The eight Boolean functions should be implemented successfully. Their outputs should match the theoretical truth tables for all input combinations.

## 8. Result
<img width="410" height="206" alt="Screenshot 2026-11-17 151122" src="https://github.com/user-attachments/assets/9708c4d5-62b9-4b7c-97e8-8673d5f566a7" />
<img width="409" height="209" alt="Screenshot 2026-11-17 151133" src="https://github.com/user-attachments/assets/6ec7aac9-4dc1-4643-b3e8-ba1d2c10d185" />
<img width="410" height="186" alt="Screenshot 2026-11-17 151144" src="https://github.com/user-attachments/assets/c72467f2-8347-4859-b40b-02ff8d60a480" />
<img width="406" height="205" alt="Screenshot 2026-11-17 151154" src="https://github.com/user-attachments/assets/efb6b086-8d66-431d-9b2b-3fdb3c6ced1b" />
<img width="409" height="199" alt="Screenshot 2026-11-17 151204" src="https://github.com/user-attachments/assets/bd90b24d-a1af-4264-9458-1f6c5716d4e0" />
<img width="407" height="218" alt="Screenshot 2026-11-17 151215" src="https://github.com/user-attachments/assets/4575f3a8-7ee4-4b25-800e-8db88342df64" />
<img width="409" height="224" alt="Screenshot 2026-11-17 151224" src="https://github.com/user-attachments/assets/fbf30b69-4ace-42a3-8424-ba137cdfe40a" />
<img width="409" height="200" alt="Screenshot 2026-11-17 151235" src="https://github.com/user-attachments/assets/41a77168-17e8-4fbf-aefd-42aac2a72552" />

The logic circuits are designed, implemented, and verified using Boolean algebra and digital logic gates. The original and simplified circuits are compared based on gate count and logic depth.

## 9. Repository Structure

```text
EXPERIMENT-01-BUILDING-LOGICAL-CIRCUITS/
├── README.md
├── circuit_diagrams/
├── truth_tables/
├── simulation_files/
└── results/
```

## 10. Viva Questions

1. What are universal logic gates?
2. State De Morgan's theorems.
3. What is the difference between SOP and POS?
4. How does XOR differ from XNOR?
5. How can Boolean expressions be simplified?
6. How many truth-table rows are required for six inputs?
7. What is logic depth?
8. Why is functional verification necessary?
