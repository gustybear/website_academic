---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "EE260: Introduction to Digital Design"

subtitle: "Spring, 2021 (Virtual)"

summary: "EE260 is the introductory course on digital circuit synthesis, focusing on the design and implementation of combinational logic, sequential logic, and basic central processor (van Neumann/Princeton architecture) through Verilog HDL and FPGA."

date: 2021-01-05T10:51:00-10:00
lastmod: 2021-01-05T10:51:00-10:00
featured: false
draft: false

authors:
- Yao Zheng
- Marionne Millan

tags:
- digital circuit
- hardware synthesis
- verilog
- fpga
- xilinx
- combinational logic
- sequential logic
- finite state machine
- high level finite state machine
- van neumann architecture
- princeton architecture
- offered course
- current semester

categories: []

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
#- name: Sample Report
#  url: ./docs/reports/course_ee693e_2020_fall/week_02/01/
#- name: Sample Report
#  url: ./docs/reports/course_ee693e_2020_fall/week_02/02/
---
***
# Executive Summary
This course explores the foundation of digital circuit design, starting from Boolean algebra, through combinational and sequential logic, to finite state machines and basic central processing units (CPUs) under von Neumann architecture. The associated laboratory segment introduces modern digital design techniques, e.g., hardware description language ([Verilog] HDL) and field-programmable gate array (FPGA), to model, implement, and test the aforementioned digital circuits.
***

# Logistics
- *Lecturer*: [Yao Zheng](mailto:yao.zheng@hawaii.edu)
- *Teaching Assistant*: [Marionne Millan](mailto:marionne@hawaii.edu)
- *Lecture*:
  - Textbook: [EE 260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021), by Zybooks.
  - Time: Mondays, Wednesdays, and Fridays 9:30am-10:20am.
  - Format: [Zoom](https://hawaii.zoom.us/j/5764842348).
- *Laboratory*:
  - Tools:
    - Software: Xilinx Vivado. 
    - Hardware: Basys 3 FPGA Trainer Board.
  - Time: 
    - Session 01: Tuesdays 9:00am-11:45am.
    - Session 02: Tuesdays 1:30pm-4:15pm.
  - Format: 
    - Session 01:
      - [Discord Server](https://discord.gg/qMKyx6PcsP)
      - [Classroom](https://classroom.google.com/c/MjUwMzMyNjE4MTk4?cjc=l4oycey)
    - Session 02:
      - [Discord Server](https://discord.gg/cfkJVUBFyN)
      - [Classroom](https://classroom.google.com/c/MjUwMzMyNjE4MjA5?cjc=e3kptgu)
- *Office hours*: see [here](../../#contact).

***
# Grading
- *Homework*: Participation and challenge problems are **different** for each student and **automatically graded** by the zyBook platform. You are encouraged to discuss homework assignments with your classmates. Discussions may include general approaches to a problem and suggested resource material. 

- *Lab reports*: Lab report, **submitted per team**, are **graded by peer teams** based on the rubric specified by the TA. All team members must attend lab, jointly demonstration their implementations, and submit a single lab report to the TA. You may discuss the general approach to the lab assignment with other teams. You are encouraged to discuss lab assignments with other teams. Discussions may include general approaches to a design and suggested resource material.

- *Exams*: All exams are strictly individual efforts. 

- *Proscribed Conduct*: Copying or otherwise cheating on homework, lab reports, or exam will result in a failing grade for the course. More details can be found at student conduct code policies, [III.C.](http://studentaffairs.manoa.hawaii.edu/policies/conduct_code/proscribed_conduct.php)

## Percentages
| Participation | Challenge | Labs           | Midterms (2) | Final |
| ----------    | ------    | -------------- | -------      | ---   |
| 5%            | 20%       | 25%            | 30%          | 20%   |

## Curves
| Linear                         | Bell            |
| ---                            | ---             |
| participation, challenge, Labs | Midterms, Final |

## Cutoffs
| A-     | B-    | C-    |
| ------ | ----- | ----- |
| 70%    | 50%   | 30%   |

***
# Schedule
## Lecture
| TIME                                     | TOPICS                                                              | READING/HW                     | HW due         |
| ---                                      | ---                                                                 | ---                            | ---            |
| [Week 1 (1/11. 1/13, 1/15)][week 01 url] | Course Logistic and Introduction                                    | [zyBooks Week 01][read 01 url] | 23:59:59, 1/17 |
| Week 2 (1/20. 1/22)                      | Number Systems                                                      | zyBooks Week 02                | 23:59:59, 1/24 |
| Week 3 (1/25. 1/27, 1/29)                | Combinational Logic: Switches, Transistors, Logic Gates             | zyBooks Week 03                | 23:59:59, 1/31 |
| Week 4 (2/1, 2/3, 2/5)                   | Combinational Logic: Boolean Algebra                                | zyBooks Week 04                | 23:59:59, 2/7  |
| Week 5 (2/8, 2/10, 2/12)                 | Combinational Logic: Design Process, More Gates                     | zyBooks Week 05                | 23:59:59, 2/14 |
| Week 6 (Feb 17)                          | Review: Combinational Logic                                         | --                             | --             |
| Week 6 (Feb 19)                          | Midterm I: 9:30AM - 10:45AM                                         | --                             | --             |
| Week 7 (2/22, 2/24, 2/26)                | Review: Midterm I, Sequential Logic: Clock, Latches, and Flip-Flops | zyBooks Week 07                | 23:59:59, 2/28 |
| Week 8 (3/1, 3/3, 3/5)                   | Sequential Logic: Finite State Machines                             | zyBooks Week 08                | 23:59:59, 3/7  |
| Week 9 (3/8, 3/10, 3/12)                 | Sequential Logic: Registers, Counters, Shifters, and Arithmetic     | zyBooks Week 09                | 23:59:59, 3/14 |
| Spring Recess (Mar 15  - Mar 19)         | --                                                                  | --                             | --             |
| Week 10 (Mar 22)                         | Review: Sequential Logic                                            | --                             | --             |
| Week 10 (Mar 24)                         | Midterm II: 9:30AM - 10:45AM                                        | --                             | --             |
| Week 11 (3/29, 3/31)                     | Review: Midterm II, Register-Transfer Level Design                  | zyBooks Week 11                | 23:59:59, 4/4  |
| Week 12 (4/5, 4/7, 4/9)                  | Register Memory Components and FIFO                                 | zyBooks Week 12                | 23:59:59, 4/11 |
| Week 13 (4/12, 4/14, 4/16)               | Optimizations and Tradeoffs                                         | zyBooks Week 13                | 23:59:59, 4/18 |
| Week 14 (4/19, 4/21, 4/23)               | Physical Implementation on ICs                                      | zyBooks Week 14                | 23:59:59, 4/25 |
| Week 15 (4/26, 4/28, 4/30)               | Programmable Processors                                             | zyBooks Week 15                | 23:59:59, 5/02 |
| Week 16 (5/3, 5/5)                       | Class Review                                                        | --                             | --             |
| Study Days (May 07, 08)                  | --                                                                  | --                             | --             |
| Week 17 (5/10)                           | Final: 9:45AM - 11:45AM                                             | --                             | --             |

## Laboratory

| TIME                                            | TOPICS                                                             | LABORATORY                                 | READING                        | ASSIGMENT                                     | DUE (before first lecture) |
| ---                                             | ---                                                                 | ---                                        | ---                            | ---                                           | ---                        |
| [Week 1 (1/11. 1/13, 1/15)]          | Course Logistic and Introduction                                    |                                            | zyBooks Week 01                |                                               | --                         |
| [Week 2 (1/20. 1/22)]              | Number Systems                                                      | Vivado Tutorial                            | zyBooks Week 02                | Numbering Systems                             | --                         |
| [Week 3 (1/25. 1/27, 1/29)]          | Combinational Logic: Switches, Transistors, Logic Gates             | Modeling Concepts                          | zyBooks Week 03                | Switches, Transistors, Logic Gates            | Week 1                     |
| [Week 4 (2/1, 2/3, 2/5)]          | Combinational Logic: Boolean Algebra                                | Numbering Systems                          | zyBooks Week 04                | Boolean Algebra                               | Week 2                     |
| [Week 5 (2/8, 2/10, 2/12)]          | Combinational Logic: Design Process, More Gates                     | Multi-Output Circuits                      | zyBooks Week 05                | Design Process, More Gates                    | Week 3                     |
| Week 6 (Feb 17)                                 | Review: Combinational Logic                                         |                                            |                                |                                               | Week 4                     |
| [Week 6 (Feb 19)]                  | Midterm I: Computer allowed.                                        | At home.                                   | 9:30AM - 10:45AM               |                                               |                            |
| [Week 7 (2/22, 2/24, 2/26)]          | Review: Midterm I, Sequential Logic: Clock, Latches, and Flip-Flops | Tasks Functions, and Testbench             | [zyBooks Week 07] | Latches and Flip-Flops                        | Week 5                     |
| [Week 8 (3/1, 3/3, 3/5)]          | Sequential Logic: Finite State Machines                             | Modeling Latches and Flip-Flops            | [zyBooks Week 08] | Finite State Machines                         | --                         |
| [Week 9 (3/8, 3/10, 3/12)]          | Sequential Logic: Registers, Counters, Shifters, and Arithmetic     | Finite State Machines                      | [zyBooks Week 09] | Registers, Counters, Shifters, and Arithmetic | Week 7                     |
| Spring Recess (Mar 15  - Mar 19)                |                                                                     |                                            |                                |                                               |
| Week 10 (Mar 22)                                | Review: Sequential Logic                                            |                                            |                                |                                               | Week 8                     |
| [Week 10 (Mar 24)]                 | Midterm Exam II:          Computer allowed.                         | At home.                                   | 9:30AM - 10:45AM               |                                               |
| [Week 11 (3/29, 3/31)] | Register-Transfer Level Design                                      | Modeling Registers and Counters            | [zyBooks Week 11] | Register-Transfer Level Process               | Week 9                     |
| [Week 12 (4/5, 4/7, 4/9)]             | Register Memory Components and FIFO                                 | Architectural Wizard and IP Catalog        | [zyBooks Week 12] | Register Files, Cache, and Memory Components  | --                         |
| [Week 13 (4/12, 4/14, 4/16)]         | Optimizations and Tradeoffs                                         | Behavioral Modeling and Timing Constraints | [zyBooks Week 13] | Optimizations and Tradeoffs                   | Week 11                    |
| [Week 14 (4/19, 4/21, 4/23))]         | Physical Implementation on ICs                                      | Sequential System Design using ASM Charts  | [zyBooks Week 14] | Physical Implementation on ICs                | Week 12                    |
| [Week 15 (4/26, 4/28, 4/30)]     | Programmable Processors                                             | Catch-up Lab                               | [zyBooks Week 15] | Programmable Processors                       | Week 13                    |
| [Week 16 (May 03, 05)]             | Class Review                                                        |                                            |                                |                                               | Week 14                    |
| Study Days (May 07, 08)                         |                                                                     |                                            |                                |                                               |
| [Week 17 (May 10)][week 17 url]                 | Final:       Computer allowed                                       | Kuykendall Hall 305                        | 9:45AM - 11:45AM               |                                               | Week 15                    |
***
# Resources
## Xilinx Vivado and Basys3 
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

### Verilog
- [Introduction to Verilog][introduction to verilog url]
- [Introduction to Verilog Video][introduction to verilog video url]

### Schemetic Drawing
- [LogicWorks][logicworks url]
- [Digikey Schemeit][digikey schemeit url]

[week urls]: # (week urls)
[week 01 url]: https://classroom.github.com/a/2va04_ad
[week 02 url]: https://classroom.github.com/a/SvtGnkD7
[week 03 url]: https://classroom.github.com/a/rFAYuj_8
[week 04 url]: https://classroom.github.com/a/UZPNuyoo
[week 05 url]: https://classroom.github.com/a/JNxgXMaM
[week 06 url]: https://classroom.github.com/a/TfhRNuDv
[week 07 url]: https://classroom.github.com/a/fIGWecjk
[week 08 url]: https://classroom.github.com/a/eeiPKFYJ
[week 09 url]: https://classroom.github.com/a/v2DQycY1
[week 10 url]: https://classroom.github.com/a/jruqU2Sl
[week 11 url]: https://classroom.github.com/a/5TDnj9SM
[week 12 url]: https://classroom.github.com/a/WyB0SkZD
[week 13 url]: https://classroom.github.com/a/76NMroe-
[week 14 url]: https://classroom.github.com/a/7tRD76MI
[week 15 url]: https://classroom.github.com/a/ym8TefFX
[week 16 url]: https://classroom.github.com/a/eqfZxWdk
[week 17 url]: https://classroom.github.com/a/ahPU1u-k

[read urls]: # (reading urls)
[read 01 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/1/section/1
[read 02 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/2/section/1
[read 03 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/3/section/1
[read 04 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/4/section/1
[read 05 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/5/section/1
[read 06 url]: # (reading urls)
[read 07 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/6/section/1
[read 08 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/7/section/1
[read 09 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/8/section/1
[read 10 url]: # (reading urls)
[read 11 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/9/section/1
[read 12 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/10/section/1
[read 13 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/11/section/1
[read 14 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/12/section/1
[read 15 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021/chapter/13/section/1
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
