# 32-bit RISC-V Processor (RTL to GDSII)

One-line summary: pipelined RV32I core in SystemVerilog,
taken through the physical design flow.

## Status
| Stage | Description | Status |
|---|---|---|
| 1 | Instruction encoding/decoding | Done |
| 2 | ALU + testbench | In progress |
| 3 | Register file | Not started |
| ... | ... | ... |

## Supported instructions
(add/sub/and/or abhi, baaki jaise jaise ban-te jaayein)

## Tools used
Icarus Verilog, GTKWave, (Cadence / OpenLane later)

## How to run
iverilog -g2012 -o alu_sim rtl/alu.sv tb/alu_tb.sv
vvp alu_sim

## Results
(timing, area, power: baad me, sirf real numbers)

## What I learned / bugs I hit
See docs/bugs_log.md
