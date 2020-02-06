+++
title = "EE260: Introduction to Digital Design"
subtitle = "Spring, 2020, updated labs"
date = 2020-01-10T00:00:00-10:00
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
authors= ["Marionne Casipit", "Anthony Gasbarro", "Yao Zheng"]
tags = ["digital design", "fpga", "current", "featured"]
+++

***
Digital circuits are the foundations to build calculators, computers and cell phones, etc. This course explores these foundations by using modern digital design techniques to design, implement and test digital circuits ranging from basic logic gates to state machines that perform useful functions like calculations, counting, timing, and a host of other applications. Students will learn modern design techniques, using a hardware description language (HDL) such as Verilog to design, simulate and implement logic systems consisting of basic gates, adders, multiplexers, latches, counters, and basic processors.

The function and operation of programmable logic devices, such as field programmable gate arrays (FPGAs), will be described and discussed in terms of how an HDL logic design is mapped and implemented. Experiments involving the design of combinational and sequential circuits will provide students a hand-on introduction to basic digital electrical engineering concepts and the skills needed to gain more advanced skills. In the laboratory, students will construct, troubleshoot, and test the digital circuits that they have developed using a hardware description language. These custom logic designs will be implemented using FPGAs and validated using test equipment.

***
## Logistics
- *Lecturer*: [Yao Zheng](mailto:yao.zheng@hawaii.edu)
- *Teaching Assistant(s)*: [Anthony Gasbarro](mailto:agasbarr@hawaii.edu)
- *Grader(s)*: [Marionne Casipit](mailto:marionne@hawaii.edu)
- *Lecture Time*: Mondays, Wednesdays, and Fridays 9:30am-10:20am, Kuykendall Hall 305.
- *Lab Time*: Tuesdays 9:00am-11:45am or 1:30pm-4:15pm, Holmes Hall 451.
- *Office hours*: see [here](../../#contact).

***
## Textbook
- *Recommended*: [EE 260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260Spring2020), by Zybooks
  - Buy at [ZyBooks](https://learn.zybooks.com/zybook/HAWAIIEE260Spring2020)
  - [How to use Zybooks](https://learn.zybooks.com/zybook/HowToUseZyBooks2)
- *Recommended*: [Digital Design Principles and Practice with Verilog (5th Edition)](https://www.pearson.com/us/higher-education/program/Wakerly-Digital-Design-Principles-and-Practices-5th-Edition/PGM337271.html), by John F. Wakerly.
  - Buy at [Amazon](https://www.amazon.com/Digital-Design-Principles-Practices-5th/dp/013446009X/ref=sr_1_1?ie=UTF8&qid=1546977313&sr=8-1&keywords=Digital+Design+Principles+and+Practice).
  - By at UHM Bookstore.
  - Library Reserve (Sinclair Library Wong Audiovisual Center, Call#: TK7874.65 .W34 2018).
- *Optional*: [Digital Design with RTL Design, VHDL, and Verilog (2nd Edition)](http://bcs.wiley.com/he-bcs/Books?action=index&itemId=0470531088&bcsId=5568), by Frank Vahid.
  - Buy at [Amazon](https://www.amazon.com/Digital-Design-RTL-VHDL-Verilog/dp/0470531088/ref=sr_1_1?keywords=Digital+Design+with+RTL+Design%2C+VHDL%2C+and+Verilog+%282nd+Edition%29&qid=1578885767&sr=8-1).
  - Library Reserve (Hamilton Library Circulation, Call # -  TK7888.3 .V274 2011).
- *Optional*: [FPGA Prototyping By Verilog Examples: Xilinx Spartan-3 Version (1st Edition)](https://academic.csuohio.edu/chu_p/rtl/fpga_vlog.html), by Pong P. Chu.
- *Optional*: [FPGA Prototyping by SystemVerilog Examples: Xilinx MicroBlaze MCS SoC Edition (2nd Edition)](https://academic.csuohio.edu/chu_p/rtl/fpga_mcs_sv.html), by Pong P. Chu.

***
## Xilinx Vivado and Basys3 
(required for lab and assignments)
- [Xilinx Vivado](https://www.xilinx.com/products/design-tools/vivado/vivado-webpack.html):
  - Access Vivado on campus computers:
    - Holmes Hall 451
    - Holmes Hall 387
  - Access Vivado on personal computers:
    - PC (Windows and Linux systems): [installation guide][xilinx vivado installation guide video url]
    - Mac (MacOS): requires a Linux virtual instance 
      - [Oracle VM VirtualBox (local, free)](https://www.virtualbox.org/): [installation guide][virtualbox guide url], [setup usb][virtualbox usb guide url]
      - [Amazon Workspaces (cloud, paid)](https://aws.amazon.com/workspaces/): [installation guide][amazon workspace guide url]
  - [Xilinx Vivado Getting Started][xilinx vivado getting started url]
- [Basys 3 FPGA Trainer Board](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
  - Access Basys 3 board on campus: 
    - Holmes Hall 451 (in-house use only)
    - Holmes Hall 483 (limited quantities , short loan, first come, fisrt served) 
  - [Basys3 Master XDC File][basys3 master xdc file url]
  - [Basys3 Reference Manual][basys3 reference manual url]
  - [Basys3 Schematic][basys3 schematic url]

***
## Grading
### Percentages
| Homework   | Labs (required) | Midterms (2)   | Final or Labs (optional) | Reading Bonus |
| ---------- | ------          | -------------- | -------                  | ---           |
| 25%        | 25%             | 30%            | 20%                      | 5%            |

### Curves
| Linear         | Bell            |
| ---            | ---             |
| Homework, Labs | Midterms, Final |

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
| TIME                                   | LECTURE                                                             | LABORATORY                                 | READING                              | ASSIGMENT                                     | DUE (before first lecture) |
| ---                                    | ---                                                                 | ---                                        | ---                                  | ---                                           | ---                        |
| [Week 1 (Jan 13, 15, 17)][week 01 url] | Course Logistic and Introduction                                    |                                            | Wakerly 1.1 - 1.12                   |                                               | --                         |
| [Week 2 (Jan 22, 24)][week 02 url]     | Number Systems                                                      | Vivado Tutorial                            | Wakerly 2.1 - 2.6, 2.10, 2.11        | Numbering Systems                             | --                         |
| [Week 3 (Jan 27, 29, 31)][week 03 url] | Combinational Logic: Switches, Transistors, Logic Gates             | Modeling Concepts                          | Wakerly 3.1, 3.2, 4.1, 5.1 - 5.3     | Switches, Transistors, Logic Gates            | Week 1                     |
| [Week 4 (Feb 03, 05, 07)][week 04 url] | Combinational Logic: Boolean Algebra                                | Numbering Systems                          | Wakerly 4.2, 4.3, 5.4                | Boolean Algebra                               | Week 2                     |
| [Week 5 (Feb 10, 12, 14)][week 05 url] | Combinational Logic: Design Process, More Gates                     | Multi-Output Circuits                      | Wakerly 6.1, 6.2, 6.4, 6.7           | Design Process, More Gates                    | Week 3                     |
| Week 6 (Feb 19)                        | Review: Combinational Logic                                         |                                            |                                      |                                               | Week 4                     |
| Week 6 (Feb 21)                        | Midterm I: Computer allowed.                                        | At home.                                   | 9:30AM - 10:20AM                     |                                               |                            |
| Week 7 (Feb 24, 26, 28)                | Review: Midterm I, Sequential Logic: Clock, Latches, and Flip-Flops | Tasks Functions, and Testbench             | Wakerly 10.1, 10.2, 10.3, 10.4       | Latches and Flip-Flops                        | Week 5                     |
| Week 8 (Mar 02, 04, 06)                | Sequential Logic: Finite State Machines                             | Modeling Latches and Flip-Flops            | Wakerly 9.1 - 9.3, 9.6, 5.14         | Finite State Machines                         | --                         |
| Week 9 (Mar 09, 11, 13)                | Sequential Logic: Registers, Counters, Shifters, and Arithmetic     | Finite State Machines                      | Wakerly 8.1 - 8.3, 7.4, 11.1, 11.2   | Registers, Counters, Shifters, and Arithmetic | Week 7                     |
| Spring Recess (Mar 16 - Mar 20)        |                                                                     |                                            |                                      |                                               |
| Week 10 (Mar 23)                       | Review: Sequential Logic                                            |                                            |                                      |                                               | Week 8                     |
| Week 10 (Mar 25)                       | Midterm Exam II:          Computer allowed.                         | At home.                                   | 9:30AM - 10:45AM                     |                                               |
| Week 10 (Mar 27)                       | Review: Midterm Exam II                                             |                                            |                                      |                                               |
| Week 11 (Mar 30, Apr 01, Apr 03)       | Register-Transfer Level Design                                      | Modeling Registers and Counters            | Wakerly 12.1 - 12.9, 13.1 - 13.3     | Register-Transfer Level Process               | Week 9                     |
| Week 12 (Apr 06, 08)                   | Register Memory Components and FIFO                                 | Sequential System Design using ASM Charts  | Wakerly 15.1 - 15.4                  | Register Files, Cache, and Memory Components  | --                         |
| Week 13 (Apr 13, 15, 17)               | Optimizations and Tradeoffs                                         | Behavioral Modeling and Timing Constraints | Wakerly 3.2, 3.4, 8.1.4 - 8.1.6 12.8 | Optimizations and Tradeoffs                   | Week 11                    |
| Week 14 (Apr 20, 22, 24)               | Physical Implementation on ICs                                      | Architectural Wizard and IP Catalog        | Wakerly 14.1 - 14.7                  | Physical Implementation on ICs                | Week 12                    |
| Week 15 (Apr 27, 29, May 01)           | Programmable Processors                                             | Catch-up Lab                               | (Optional) Vahid 8.1 - 8.5           | Programmable Processors                       | Week 13                    |
| Week 16 (May 04, 06)                   | Class Review                                                        |                                            |                                      |                                               | Week 14                    |
| Study Days (May 08, 09)                |                                                                     |                                            |                                      |                                               |
| Week 17 (May 11)                       | Final:       Computer allowed                                       | Kuykendall Hall 305                        | 9:45AM - 11:45AM                     |                                               | Week 15                    |

***
## Resources
### Verilog
- [Introduction to Verilog][introduction to verilog url]
- [Introduction to Verilog Video][introduction to verilog video url]

### Schemetic Drawing
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
[week 01 url]: https://classroom.github.com/a/2va04_ad
[week 02 url]: https://classroom.github.com/a/SvtGnkD7
[week 03 url]: https://classroom.github.com/a/rFAYuj_8
[week 04 url]: https://classroom.github.com/a/UZPNuyoo
[week 05 url]: https://classroom.github.com/a/JNxgXMaM
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

[read urls]: # (reading urls)
[read 01 url]: # (reading urls)
[read 02 url]: # (reading urls)
[read 03 url]: # (reading urls)
[read 04 url]: # (reading urls)
[read 05 url]: # (reading urls)
[read 06 url]: # (reading urls)
[read 07 url]: # (reading urls)
[read 08 url]: # (reading urls)
[read 09 url]: # (reading urls)
[read 10 url]: # (reading urls)
[read 11 url]: # (reading urls)
[read 12 url]: # (reading urls)
[read 13 url]: # (reading urls)
[read 14 url]: # (reading urls)
[read 15 url]: # (reading urls)
[read 16 url]: # (reading urls)
[read 17 url]: # (reading urls)

[resource urls]: # (resource urls)
[xilinx vivado installation guide url]: ./tutorials/xilinx_vivado_installation_guide/
[virtualbox guide url]: https://www.youtube.com/watch?v=RH1alY-MX_U
[virtualbox usb guide url]: https://www.centennialsoftwaresolutions.com/post/connecting-vivado-to-digilent-s-usb-to-jtag-through-virtualbox
[amazon workspace guide url]: https://aws.amazon.com/blogs/aws/new-amazon-linux-workspaces/
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
