# Parameterized N-Bit ALU (SystemVerilog)

A synthesizable, parameterized **N-bit Arithmetic Logic Unit (ALU)** written in SystemVerilog with Zero, Carry, and signed Overflow status flags, verified using a self-checking testbench.

## Supported Operations (`op[2:0]`)
| Opcode | Operation | Description |
| :--- | :--- | :--- |
| `000` | `ADD` | Unsigned/signed addition (`a + b`) |
| `001` | `SUB` | Subtraction (`a - b`) |
| `010` | `AND` | Bitwise AND (`a & b`) |
| `011` | `OR` | Bitwise OR (`a \| b`) |
| `100` | `XOR` | Bitwise XOR (`a ^ b`) |
| `101` | `NOT` | Bitwise inversion (`~a`) |
| `110` | `SHL` | Logical shift left by 1 (`a << 1`) |
| `111` | `SHR` | Logical shift right by 1 (`a >> 1`) |

## Repository Structure
- `rtl/alu.sv` — Synthesizable SystemVerilog ALU design
- `tb/alu_tb.sv` — Self-checking testbench with directed and randomized stimulus
- `docs/` — Simulation waveform screenshots
