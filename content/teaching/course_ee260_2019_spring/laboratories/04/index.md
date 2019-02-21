---
title: "Laboratory 04: Tasks, Functions, and Testbench"
subtitle: "EE260: Introduction to Digital Design"
date: 2018-12-01T17:21:22-10:00
resources:
- src: 'images/basys3.png'
  name: Basys3
---
## Github Classroom
Accept your laboratory assignment [here](TBD).

## Introduction
Verilog lets you define sub-programs using tasks and functions. They are used to improve the readability
and to exploit re-usability code. Functions are equivalent to combinatorial logic and cannot be used to
replace code that contains event or delay control operators (as used in a sequential logic). Tasks are
more general than functions, and may contain timing controls. Testbench is a program or model written in
any language for the purposes of exercising and verifying the functional correctness of a hardware model
during the simulation. Verilog is primarily a means for hardware modeling (simulation), the language
contains various resources for formatting, reading, storing, allocating dynamically, comparing, and writing
simulation data, including input stimulus and output results.

In this lab, you will learn how to write tasks, functions, and testbenches. You will learn about the
components of a testbench, and language constructs available to verify the correctness of the underlying
hardware model. Please refer to the Vivado tutorial on how to use the Vivado tool for creating projects and verifying digital circuits.

## Objectives
After completing this lab, you will be able to:

- Develop tasks for modeling a combinatorial circuit

- Develop functions for modeling a combinatorial circuit

- Develop a testbench to test and validate a design under test

## Full Description

Full description of the lab can be found [here](https://www.xilinx.com/support/documentation/university/Vivado-Teaching/HDL-Design/2015x/Verilog/docs-pdf/lab4.pdf).
