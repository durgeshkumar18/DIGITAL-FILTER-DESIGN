# CODTECH Internship Project  
## FIR (Finite Impulse Response) Filter - Verilog Design

**Intern Name**: [Durgesh Kumar Nishad]  
**Internship Domain**: VLSI Design  
**Company**: CODTECH IT SOLUTIONS  
**Project Title**: Digital FIR Filter Design using Verilog  
**Completion Date**: [20/4/2025]  

---

## Description

This project implements a basic FIR Filter using Verilog. The filter processes signed 8-bit inputs and uses 4 fixed coefficients to compute output samples synchronously.

---

## Files Included

| File Name         | Description                                |
|------------------|--------------------------------------------|
| `fir_filter.v`    | FIR filter RTL design in Verilog           |
| `tb_fir_filter.v` | Testbench with input samples               |
| `fir_wave.vcd`    | Waveform file for GTKWave visualization    |
| `README.md`       | Documentation with performance summary     |

---

## Filter Design Parameters

- **Filter Type**: Low-pass FIR filter  
- **Taps**: 4  
- **Input Bit Width**: 8-bit signed  
- **Output Bit Width**: 18-bit  
- **Coefficients**: {3, 5, 5, 3}  

---

## Simulation

### Run using Icarus Verilog:
```bash
iverilog -o fir_test tb_fir_filter.v fir_filter.v
vvp fir_test
gtkwave fir_wave.vcd# DIGITAL-FILTER-DESIGN
