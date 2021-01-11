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
- **Personnel**:
  - Lecturer: [Yao Zheng](mailto:yao.zheng@hawaii.edu)
    - Office hours: see [here](../../#contact).
  - TA: [Marionne Millan](mailto:marionne@hawaii.edu)
    - Office Hours: 
- **Lecture**:
  - Textbook: [EE 260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021), by Zybooks.
  - Time: Mondays, Wednesdays, and Fridays 9:30am-10:20am.
  - Format: [Zoom](https://hawaii.zoom.us/j/5764842348).
- **Laboratory**:
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
  - Software: [Xilinx Vivado](https://www.xilinx.com/products/design-tools/vivado/vivado-webpack.html). 
    - PC (Windows and Linux systems): [installation guide][xilinx vivado installation guide video url]
    - Mac (MacOS): requires a Linux virtual instance 
      - [Oracle VM VirtualBox (local, free)](https://www.virtualbox.org/): [installation guide][virtualbox guide url]
      - [Amazon Workspaces (cloud, paid)](https://aws.amazon.com/workspaces/): [installation guide][amazon workspace guide url]
  - Hardware: Basys 3 FPGA Trainer Board
    - Pick up at Holme Hall 488 on 1/13, 2:00PM (limited quantities, first come, fisrt served).
    - Buy at [Digilent](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/).

***
# Grading
- **Homework**: Participation and challenge problems are **different** for each student and **automatically graded** by the zyBook platform. You are encouraged to discuss homework assignments with your classmates. Discussions may include general approaches to a problem and suggested resource material. 

- **Lab reports**: Lab report, **submitted per team**, are **graded by peer teams** based on the rubric specified by the TA. All team members must attend lab, jointly demonstration their implementations, and submit a single lab report to the TA. You may discuss the general approach to the lab assignment with other teams. You are encouraged to discuss lab assignments with other teams. Discussions may include general approaches to a design and suggested resource material.

- **Exams**: All exams are strictly individual efforts. 

- **Percentages**
| Participation | Challenge | Labs           | Midterms (2) | Final |
| ----------    | ------    | -------------- | -------      | ---   |
| 5%            | 20%       | 25%            | 30%          | 20%   |

- **Curves**
| Linear                         | Bell            |
| ---                            | ---             |
| participation, challenge, Labs | Midterms, Final |

- **Cutoffs**
| A-     | B-    | C-    |
| ------ | ----- | ----- |
| 70%    | 50%   | 30%   |

- **Proscribed Conduct**: Copying or otherwise cheating on homework, lab reports, or exam will result in a failing grade for the course. More details can be found at student conduct code policies, [III.C.](http://studentaffairs.manoa.hawaii.edu/policies/conduct_code/proscribed_conduct.php)

***
# Schedule
## Lecture
| TIME                                     | TOPICS                                                              | READING/HW             | DEADLINE      |
| ---                                      | ---                                                                 | ---                    | ---           |
| [Week 1 (1/11. 1/13, 1/15)][week 01 url] | Course Logistic and Introduction                                    | [Week 01][read 01 url] | 1/17, 11:59PM |
| Week 2 (1/20. 1/22)                      | Number Systems                                                      | Week 02                | 1/24, 11:59PM |
| Week 3 (1/25. 1/27, 1/29)                | Combinational Logic: Switches, Transistors, Logic Gates             | Week 03                | 1/31, 11:59PM |
| Week 4 (2/1, 2/3, 2/5)                   | Combinational Logic: Boolean Algebra                                | Week 04                | 2/7, 11:59PM  |
| Week 5 (2/8, 2/10, 2/12)                 | Combinational Logic: Design Process, More Gates                     | Week 05                | 2/14, 11:59PM |
| Week 6 (Feb 17)                          | Review: Combinational Logic                                         | --                     | --            |
| Week 6 (Feb 19)                          | Midterm I: 9:30AM - 10:45AM                                         | --                     | --            |
| Week 7 (2/22, 2/24, 2/26)                | Review: Midterm I, Sequential Logic: Clock, Latches, and Flip-Flops | Week 07                | 2/28, 11:59PM |
| Week 8 (3/1, 3/3, 3/5)                   | Sequential Logic: Finite State Machines                             | Week 08                | 3/7, 11:59PM  |
| Week 9 (3/8, 3/10, 3/12)                 | Sequential Logic: Registers, Counters, Shifters, and Arithmetic     | Week 09                | 3/14, 11:59PM |
| Spring Recess (Mar 15  - Mar 19)         | --                                                                  | --                     | --            |
| Week 10 (Mar 22)                         | Review: Sequential Logic                                            | --                     | --            |
| Week 10 (Mar 24)                         | Midterm II: 9:30AM - 10:45AM                                        | --                     | --            |
| Week 11 (3/29, 3/31)                     | Review: Midterm II, Register-Transfer Level Design                  | Week 11                | 4/4, 11:59PM  |
| Week 12 (4/5, 4/7, 4/9)                  | Register Memory Components and FIFO                                 | Week 12                | 4/11, 11:59PM |
| Week 13 (4/12, 4/14, 4/16)               | Optimizations and Tradeoffs                                         | Week 13                | 4/18, 11:59PM |
| Week 14 (4/19, 4/21, 4/23)               | Physical Implementation on ICs                                      | Week 14                | 4/25, 11:59PM |
| Week 15 (4/26, 4/28, 4/30)               | Programmable Processors                                             | Week 15                | 5/02, 11:59PM |
| Week 16 (5/3, 5/5)                       | Class Review                                                        | --                     | --            |
| Study Days (May 07, 08)                  | --                                                                  | --                     | --            |
| Week 17 (5/10)                           | Final: 9:45AM - 11:45AM                                             | --                     | --            |

## Laboratory
| TIME                    | Topic                                      | Submissions              | DEADLINE      |
| ---                     | ---                                        | ---                      | ---           |
| Week 1 (1/12)           | --                                         | ---                      | ---           |
| Week 2 (1/19)           | Vivado Tutorial                            | [Lab 01, Sec. 1][labS1 01 sub url], [Lab 01, Sec. 2][labS1 01 sub url] | 1/24, 11:59PM |
| Week 3 (1/26)           | Modeling Concepts                          | [Lab 02, Sec. 1][labS1 02 sub url], [Lab 02, Sec. 2][labS1 02 sub url] | 1/31, 11:59PM |
| Week 4 (2/2)            | Numbering Systems                          | [Lab 03, Sec. 1][labS1 03 sub url], [Lab 03, Sec. 2][labS1 03 sub url] | 2/7, 11:59PM  |
| Week 5 (2/9)            | Multi-Output Circuits                      | [Lab 04, Sec. 1][labS1 04 sub url], [Lab 04, Sec. 2][labS1 04 sub url]  2/21, 11:59PM |
| Week 6 (2/16)           | --                                         | ---                      | ---           |
| Week 7 (2/23)           | Tasks Functions, and Testbench             | [Lab 05, Sec. 1][labS1 05 sub url], [Lab 05, Sec. 2][labS1 05 sub url] | 2/28, 11:59PM |
| Week 8 (3/2)            | Modeling Latches and Flip-Flops            | [Lab 06, Sec. 1][labS1 06 sub url], [Lab 06, Sec. 2][labS1 06 sub url] | 3/7, 11:59PM  |
| Week 9 (3/9)            | Finite State Machines                      | [Lab 07, Sec. 1][labS1 07 sub url], [Lab 07, Sec. 2][labS1 07 sub url] | 3/14, 11:59PM |
| Spring Recess (3/16)    | --                                         | ---                      | ---           |
| Week 10 (3/23)          | --                                         | ---                      | ---           |
| Week 11 (3/30)          | Modeling Registers and Counters            | [Lab 08, Sec. 1][labS1 08 sub url], [Lab 08, Sec. 2][labS1 08 sub url] | 4/4, 11:59PM  |
| Week 12 (4/6)           | Architectural Wizard and IP Catalog        | [Lab 09, Sec. 1][labS1 09 sub url], [Lab 09, Sec. 2][labS1 09 sub url] | 4/10, 11:59PM |
| Week 13 (4/13)          | Behavioral Modeling and Timing Constraints | [Lab 10, Sec. 1][labS1 10 sub url], [Lab 10, Sec. 2][labS1 10 sub url] | 4/18, 11:59PM |
| Week 14 (4/20)          | Sequential System Design using ASM Charts  | [Lab 11, Sec. 1][labS1 11 sub url], [Lab 11, Sec. 2][labS1 11 sub url] | 4/25, 11:59PM |
| Week 15 (4/27)          | Catch-up Lab                               |                          | 5/2, 11:59PM  |
| Week 16 (4/4)           | --                                         | ---                      | ---           |
| Study Days (May 07, 08) | --                                         | ---                      | ---           |
| Week 17 (May 10)        | --                                         | ---                      | ---           |

***
# Resources
## Xilinx Vivado and Basys3 
- [Xilinx Vivado](https://www.xilinx.com/products/design-tools/vivado/vivado-webpack.html):
  - [Xilinx Vivado Getting Started][xilinx vivado getting started url]
- [Basys 3 FPGA Trainer Board](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
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
[week 01 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_01_slides.pdf
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

[labsS1 sub urls]: # (labs sub urls)
[labS1 01 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjUxODAxMjY0OTY2/details
[labS1 02 sub url]: # (labs sub urls)
[labS1 03 sub url]: # (labs sub urls)
[labS1 04 sub url]: # (labs sub urls)
[labS1 05 sub url]: # (labs sub urls)
[labS1 06 sub url]: # (labs sub urls)
[labS1 07 sub url]: # (labs sub urls)
[labS1 08 sub url]: # (labs sub urls)
[labS1 09 sub url]: # (labs sub urls)

[labsS2 sub urls]: # (labs sub urls)
[labS2 01 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/MjUxODI5NjI2OTgx/details
[labS2 02 sub url]: # (labs sub urls)
[labS2 03 sub url]: # (labs sub urls)
[labS2 04 sub url]: # (labs sub urls)
[labS2 05 sub url]: # (labs sub urls)
[labS2 06 sub url]: # (labs sub urls)
[labS2 07 sub url]: # (labs sub urls)
[labS2 08 sub url]: # (labs sub urls)
[labS2 09 sub url]: # (labs sub urls)

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
