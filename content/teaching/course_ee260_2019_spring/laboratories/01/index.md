---
title: "Laboratory 01: Modeling Concepts"
subtitle: "EE260: Introduction to Digital Design"
date: 2018-12-01T17:21:22-10:00
resources:
- src: 'images/basys3.png'
  name: Basys3
---
## Github Classroom
Accept your laboratory assignment [here](TBD).

## Introduction
Verilog HDL modeling language supports three kinds of modeling styles: gate-level, dataflow, and behavioral. The gate-level and dataflow modeling are used to model combinatorial circuits whereas the behavioral modeling is used for both combinatorial and sequential circuits. This lab illustrates the use of all three types of modeling by creating simple combinatorial circuits targeting Basys3 and Nexys4 DDR boards and using the Vivado 2015.1 software tool. Please refer to the Vivado tutorial on how to use the Vivado tool for creating projects and verifying digital circuits.

The Basys3 board has the following features:

  - 1,800 Kbits of fast block RAM
  - 33,280 logic cells in 5200 slices (each slice contains four 6-input LUTs and 8 flip-flops)
  - Five clock management tiles, each with a phase-locked loop (PLL)
  - 90 DSP slices
  - Internal clock speeds exceeding 450MHz
  - On-chip analog-to-digital converter (XADC)
  - 16 User Switches
  - 16 User LEDs
  - 5 User Pushbuttons
  - 4-digit 7-segment display
  - Three Pmod connectors
  - Pmod for XADC signals
  - 12-bit VGA output
  - USB-UART Bridge
  - Serial Flash
  - Digilent USB-JTAG port for FPGA programming and communication
  - USB HID Host for mice, keyboards and memory sticks

The [Basys3 board](images/basys3.png) is shown below.

{{< imgproc Basys3 Resize "500x" >}}Basys3 Board{{< /imgproc >}}

## Objectives

After completing this lab, you will be able to:

- Create scalar and wide combinatorial circuits using gate-level, dataflow, and behavioral modeling

- Write models to read switches and push buttons, and output on LEDs and 7-segment displays

- Simulate and understand the design output

- Create hierarchical designs

- Synthesize, implement and generate bitstreams

- Download bitstreams into the board and verify functionality

## Full Description

Full description of the lab can be found [here](https://www.xilinx.com/support/documentation/university/Vivado-Teaching/HDL-Design/2015x/Verilog/docs-pdf/lab1.pdf).
