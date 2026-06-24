# Full Adder and 4-bit Ripple Carry Adder
Structural RTL implementation of a Full Adder and 4-bit Ripple Carry Adder in Verilog HDL.
## Design Hierarchy
rca_4bit

└── full_adder (x4)

└── half_adder (x2)
## Files

| File | Description |
|------|-------------|
| half_adder.v | Half Adder using XOR and AND gates |
| full_adder.v | Full Adder built from two Half Adders |
| rca_4bit.v | 4-bit RCA built from four Full Adders |
| tb_half_adder.v | Testbench for Half Adder |
| tb_full_adder.v | Testbench for Full Adder |
| tb_rca_4bit.v | Testbench for 4-bit RCA |

## Simulation

```bash
iverilog -o rca_sim half_adder.v full_adder.v rca_4bit.v tb_rca_4bit.v
vvp rca_sim
gtkwave rca.vcd
```

## Tools
- Verilog HDL
- Icarus Verilog
- GTKWave
- VS Code
