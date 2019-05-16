+++
title = "EE260: Introduction to Digital Design"
subtitle = "Spring, 2019, new labs"
date = 2018-12-01T00:00:00-10:00
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["digital design", "fpga", "current", "featured"]
+++

***
Digital circuits are the foundations to build calculators, computers and cell phones, etc. This course explores these foundations by using modern digital design techniques to design, implement and test digital circuits ranging from basic logic gates to state machines that perform useful functions like calculations, counting, timing, and a host of other applications. Students will learn modern design techniques, using a hardware description language (HDL) such as Verilog to design, simulate and implement logic systems consisting of basic gates, adders, multiplexers, latches, counters, and basic processors.

The function and operation of programmable logic devices, such as field programmable gate arrays (FPGAs), will be described and discussed in terms of how an HDL logic design is mapped and implemented. Experiments involving the design of combinational and sequential circuits will provide students a hand-on introduction to basic digital electrical engineering concepts and the skills needed to gain more advanced skills. In the laboratory, students will construct, troubleshoot, and test the digital circuits that they have developed using a hardware description language. These custom logic designs will be implemented using FPGAs and validated using test equipment.

***
## Textbook
- *Required*: [Digital Design Principles and Practice with Verilog (5th Edition)](https://www.pearson.com/us/higher-education/program/Wakerly-Digital-Design-Principles-and-Practices-5th-Edition/PGM337271.html), by John F. Wakerly.
  - Buy at [Amazon](https://www.amazon.com/Digital-Design-Principles-Practices-5th/dp/013446009X/ref=sr_1_1?ie=UTF8&qid=1546977313&sr=8-1&keywords=Digital+Design+Principles+and+Practice).
  - By at UHM Bookstore (currently out of stock).
  - Interactive Digital Access Program (not available).
  - Library Reserve (Sinclair Library Wong Audiovisual Center, Call#: TK7874.65 .W34 2018).
- *Recommended*: [Digital Design with RTL Design, VHDL, and Verilog (2nd Edition)](http://bcs.wiley.com/he-bcs/Books?action=index&itemId=0470531088&bcsId=5568), by Frank Vahid.
  - Library Reserve (Sinclair Library Wong Audiovisual Center, Call#: TK7888.3 .V274 2011).
- *Optional*: [FPGA Prototyping By Verilog Examples: Xilinx Spartan-3 Version (1st Edition)](https://academic.csuohio.edu/chu_p/rtl/fpga_vlog.html), by Pong P. Chu.
- *Optional*: [FPGA Prototyping by SystemVerilog Examples: Xilinx MicroBlaze MCS SoC Edition (2nd Edition)](https://academic.csuohio.edu/chu_p/rtl/fpga_mcs_sv.html), by Pong P. Chu.

***
## Logistics
- *Lecturer*: [Yao Zheng](mailto:yao.zheng@hawaii.edu)
- *Teaching Assistant(s)*: [Matthew Iwane](mailto:iwanems@hawaii.edu), [Sasha
  Yamada](mailto:ssyamada@hawaii.edu)
- *Grader(s)*: [Kelly Ngo](mailto:kellyngo@hawaii.edu)
- *Lecture Time*: Mondays, Wednesdays, and Fridays 9:30am-10:20am, Kuykendall Hall 306.
- *Lab Time*: Tuesdays 9:00am-11:45am, Holmes Hall 451.
- *Office hours*: see [here](../../#contact).
- [*Github Organization*][github organization url]

***
## Grading
### Percentages
| Homework | Labs | Midterms (2) | Final |
|----------|------|--------------|-------|
| 25%      | 25%  | 30%          | 20%   |

### Cutoffs
| A-     | B-    | C-    |
| ------ | ----- | ----- |
| 70%    | 50%   | 30%   |

### Policies
- *Homework*: You are encouraged to discuss homework assignments with your classmates and the course staff. Discussions may include general approaches to a problem, suggested resource material and whether your final answer is correct or not. However, each student must hand in their own implementation of the homework. **Copying of homework or code will result in a grade of zero for all parties involved**.

- *Labs*: In the lab you may work in teams of two. You may discuss the general approach to the lab assignment with other teams. However, each team must implement their own solution to the lab. Both team members must attend lab and sign-off. Each team must complete any pre-lab assignments individually and must submit them with their teams lab report. Duplication of code and/or data among teams will result in a grade of zero for all students involved.

- *Exams*: All exams are strictly individual efforts. Copying or otherwise cheating on an exam will result in a failing grade for the course.

- *Proscribed Conduct*: Refer to Student Conduct Code Policies,
  [III.C.](http://studentaffairs.manoa.hawaii.edu/policies/conduct_code/proscribed_conduct.php)

***
## Schedule
| TIME                                      | LECTURE                                                         | LABORATORY                                 | READING                              | ASSIGMENT                                     | DUE (before first lecture) |
| ---                                       | ---                                                             | ---                                        | ---                                  | ---                                           | ---                        |
| [Week 1 (Jan 7, 9, 11)][week 01 url]      | Course Logistic and Introduction                                | Vivado Tutorial (optional)                 | Wakerly 1.1 - 1.12                   |                                               | --                         |
| [Week 2 (Jan 14, 16, 18)][week 02 url]    | Number Systems                                                  | Modeling Concepts                          | Wakerly 2.1 - 2.6, 2.10, 2.11        | Numbering Systems                             | --                         |
| [Week 3 (Jan 23, 25)][week 03 url]        | Combinational Logic: Switches, Transistors, Logic Gates         | Numbering Systems                          | Wakerly 3.1, 3.2, 4.1, 5.1 - 5.3     | Switches, Transistors, Logic Gates            | Week 1                     |
| [Week 4 (Jan 28, 30, Feb 1)][week 04 url] | Combinational Logic: Boolean Algebra                            | Tasks Functions, and Testbench             | Wakerly 4.2, 4.3, 5.4                | Boolean Algebra                               | Week 2                     |
| [Week 5 (Feb 4, 6, 8)][week 05 url]       | Combinational Logic: Design Process, More Gates                 | Multi-Output Circuits                      | Wakerly 6.1, 6.2, 6.4, 6.7           | Design Process, More Gates                    | Week 3                     |
| Week 6 (Feb 11)                           | Review: Combinational Logic                                     |                                            |                                      |                                               | Week 4                     |
| [Week 6 (Feb 13)][week 06 url]            | Midterm I: Computer allowed.                                    | At home.                                   | 9:30AM - 10:20AM                     |                                               |                            |
| Week 6 (Feb 15)                           | Review: Midterm I                                               |                                            |                                      |                                               |                            |
| [Week 7 (Feb 20, 22)][week 07 url]        | Sequential Logic: Clock, Latches, and Flip-Flops                | Catch-Up Lab                               | Wakerly 10.1, 10.2, 10.3, 10.4       | Latches and Flip-Flops                        | Week 5                     |
| [Week 8 (Feb 25, 27, Mar 1)][week 08 url] | Sequential Logic: Finite State Machines                         | Modeling Latches and Flip-Flops            | Wakerly 9.1 - 9.3, 9.6, 5.14         | Finite State Machines                         | Catch-Up Lab               |
| [Week 9 (Mar 4, 6, 8)][week 09 url]       | Sequential Logic: Registers, Counters, Shifters, and Arithmetic | Finite State Machines                      | Wakerly 8.1 - 8.3, 7.4, 11.1, 11.2   | Registers, Counters, Shifters, and Arithmetic | Week 7                     |
| Week 10 (Mar 11)                          | Review: Sequential Logic                                        |                                            |                                      |                                               | Week 8                     |
| [Week 10 (Mar 13)][week 10 url]           | Midterm Exam II:          Computer allowed.                     | At home.                                   | 9:30AM - 10:45AM                     |                                               |
| Week 10 (Mar 15)                          | Review: Midterm Exam II                                         |                                            |                                      |                                               |
| Spring Recess (Mar 18 - Mar 22)           |                                                                 |                                            |                                      |                                               |
| [Week 11 (Mar 25, 27, 29)][week 11 url]   | Register-Transfer Level Design                                  | No Lab (Prince Kūhiō Day)                  | Wakerly 12.1 - 12.9, 13.1 - 13.3     | Register-Transfer Level Process               | Week 9                     |
| [Week 12 (Apr 1, 3, 5)][week 12 url]      | Register Memory Components and FIFO                             | Modeling Registers and Counters            | Wakerly 15.1 - 15.4                  | Register Files, Cache, and Memory Components  | --                         |
| [Week 13 (Apr 8, 10, 12)][week 13 url]    | Optimizations and Tradeoffs                                     | Architectural Wizard and IP Catalog        | Wakerly 3.2, 3.4, 8.1.4 - 8.1.6 12.8 | Optimizations and Tradeoffs                   | Week 11                    |
| [Week 14 (Apr 15, 17)][week 14 url]       | Physical Implementation on ICs                                  | Behavioral Modeling and Timing Constraints | Wakerly 14.1 - 14.7                  | Physical Implementation on ICs                | Week 12                    |
| [Week 15 (Apr 22, 24, 26)][week 15 url]   | Programmable Processors                                         | Sequential System Design using ASM Charts  | (Optional) Vahid 8.1 - 8.5                             | Programmable Processors     | Week 13                    |
| [Week 16 (Apr 29, May 1)][week 16 url]    | Class Review                                                    |                                            |                                      |                                               | Week 14                    |
| Study Days (May 3 - May 4)                |                                                                 |                                            |                                      |                                               |
| [Week 17 (May 10)][week 17 url]           | Final:       Computer allowed                                   | Kuykendall Hall 306                        | 9:45AM - 11:45AM                     |                                               | Week 15                    |

***
## Resources
### Xilinx Vivado and Basys3
- [Xilinx Vivado HL Webpack Installation Guide][xilinx vivado installation guide url]
- [Xilinx Vivado Installation Guide Video][xilinx vivado installation guide video url]
- [Xilinx Vivado Getting Started][xilinx vivado getting started url]
- [Basys3 Master XDC File][basys3 master xdc file url]
- [Basys3 Reference Manual][basys3 reference manual url]
- [Basys3 Schematic][basys3 schematic url]

### Verilog
- [Introduction to Verilog][introduction to verilog url]
- [Introduction to Verilog Video][introduction to verilog video url]

### Schemetic
- [LogicWorks][logicworks url]
- [Digikey Schemeit][digikey schemeit url]

### Git and Github
- [Git Handbook][git handbook url]
- [GitHub Guides][github guides url]
- [GitHub Video Guides][github video guides url]
- [Github Notifications][github notification guide url]
- [Coursera: Version Control with Git][coursera git url]

### Markdown
- [Markdown Cheatsheet][markdown cheatsheet url]

### Latex
- [Latex Web Editor][latex web editor url]

### Atom (an text editor from Github, based on Electron, good for beginner)
- [Atom][atom url]
- [Atom Github Integration][atom github url]
- [Atom Markdown Enhanced Package][atom markdown enhanced url]

[github organization url]: https://github.com/ee260-spring-2019

[week urls]: # (week urls)
[week 01 url]: https://classroom.github.com/a/gT51XkDU
[week 02 url]: https://classroom.github.com/a/myEwkEY-
[week 03 url]: https://classroom.github.com/a/Yyv2H3n0
[week 04 url]: https://classroom.github.com/a/I6Q2POTP
[week 05 url]: https://classroom.github.com/a/Qhha9CyL
[week 06 url]: https://classroom.github.com/a/koXcFGC9
[week 07 url]: https://classroom.github.com/a/UUsKvNUw
[week 08 url]: https://classroom.github.com/a/5hxKW_da
[week 09 url]: https://classroom.github.com/a/M91A9VTY
[week 10 url]: https://classroom.github.com/a/ZnoDY9w3
[week 11 url]: https://classroom.github.com/a/u2FsIKRT
[week 12 url]: https://classroom.github.com/a/BGhAl8O7
[week 13 url]: https://classroom.github.com/a/K_K1nsp0
[week 14 url]: https://classroom.github.com/a/9qD4uyKa
[week 15 url]: https://classroom.github.com/a/xSlmQGOK
[week 16 url]: https://classroom.github.com/a/zMuen4fM
[week 17 url]: https://classroom.github.com/a/gEE1VsFm


[resource urls]: # (resource urls)
[xilinx vivado installation guide url]: ./tutorials/xilinx_vivado_installation_guide/
[xilinx vivado installation guide video url]: https://www.xilinx.com/video/hardware/vivado-design-suite-installation-overview.html
[xilinx vivado getting started url]: https://reference.digilentinc.com/vivado/getting_started/start
[basys3 master xdc file url]: https://www.xilinx.com/support/documentation/university/Vivado-Teaching/HDL-Design/2015x/Basys3/Supporting%20Material/Basys3_Master.xdc
[basys3 reference manual url]: https://www.xilinx.com/support/documentation/university/Vivado-Teaching/HDL-Design/2015x/Basys3/Supporting%20Material/Basys3_RM.pdf
[basys3 schematic url]: https://www.xilinx.com/support/documentation/university/Vivado-Teaching/HDL-Design/2015x/Basys3/Supporting%20Material/basys_3_sch.pdf

[introduction to verilog url]: http://vol.verilog.com/
[introduction to verilog video url]: https://www.youtube.com/watch?v=q1QwC3YlHG0

[logicworks url]: https://designworkssolutions.com/logicworks/
[digikey schemeit url]: https://www.digikey.com/schemeit/

[git handbook url]: https://guides.github.com/introduction/git-handbook/
[github guides url]: https://guides.github.com/
[github video guides url]: https://www.youtube.com/githubguides
[github notification guide url]: https://help.github.com/articles/about-notifications/
[coursera git url]: https://www.coursera.org/learn/version-control-with-git/home/welcome

[markdown cheatsheet url]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

[latex web editor url]: https://www.codecogs.com/latex/eqneditor.php

[atom url]: https://atom.io/
[atom github url]: https://github.atom.io/
[atom markdown enhanced url]: https://atom.io/packages/markdown-preview-enhanced
