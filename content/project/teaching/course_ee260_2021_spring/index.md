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
|                                                    |                                             |
| ----                                               | ---                                         |
| Lecturer: [Yao Zheng](mailto:yao.zheng@hawaii.edu) | Office Hours: see [here](../../../#contact) |
| TA: [Marionne Millan](mailto:marionne@hawaii.edu)  | Office Hours: Tues. 11:45am-12:45pm, 4:15-5:15pm |

- **Lecture**:
| Time               | Location                                    | Textbook                                                                                             | Homework Effort | Exam Effort |
| ----               | ---                                         | ---                                                                                                  | ---             | ---         |
| MWF 9:30am-10:20am | [Zoom](https://hawaii.zoom.us/j/5764842348) | [EE260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021) | Individual      | Individual  |

- **Laboratory**:
| Session | Time             | Location                                                                                                                  | Report Effort |
| ---     | ----             | ---                                                                                                                       | ---           |
| 01      | T 9:00am-11:45am | [Discord](https://discord.gg/qMKyx6PcsP), [Google Classroom](https://classroom.google.com/c/MjUwMzMyNjE4MTk4?cjc=l4oycey) | Group         |
| 02      | T 1:30pm-4:15pm  | [Discord](https://discord.gg/cfkJVUBFyN), [Google Classroom](https://classroom.google.com/c/MjUwMzMyNjE4MjA5?cjc=e3kptgu) | Group         |

***
# Grading

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
| TIME                                                                                        | TOPICS                                                                       | READING/HW                                                                 | DEADLINE      |
| ---                                                                                         | ---                                                                          | ---                                                                        | ---           |
| Week 1 ([1/13][recording 0113 url], [1/15][recording 0115 url])                             | [Course Logistic and Introduction][week 01 url]                              | [Week 01][read 01 url]                                                     | 1/17, 11:59PM |
| Week 2 ([1/20][recording 0120 url], [1/22][recording 0122 url])                             | [Number Systems][week 02 url]                                                | [Week 02][read 02 url]                                                     | 1/24, 11:59PM |
| Week 3 ([1/25][recording 0125 url], [1/27][recording 0127 url], [1/29][recording 0129 url]) | [Combinational Logic: Switches, Transistors, Logic Gates][week 03 url]       | [Week 03][read 03 url]                                                     | 1/31, 11:59PM |
| Week 4 ([2/1][recording 0201 url], [2/3][recording 0203 url], [2/5][recording 0205 url])    | [Combinational Logic: Boolean Algebra][week 04 url]                          | [Week 04][read 04 url]                                                     | 2/7, 11:59PM  |
| Week 5 ([2/8][recording 0208 url], [2/10][recording 0210 url], [2/12][recording 0212 url])  | [Combinational Logic: Design Process, More Gates][week 05 url]               | [Week 05][read 05 url]                                                     | 2/14, 11:59PM |
| Week 6 ([2/17][recording 0217 url])                                                         | [Practice Midterm I][week 06 practice url]                                   | [S1][week 06 practice submit url S1], [S2][week 06 practice submit url S2] | --            |
| Week 6 ([2/19, sol][week 06 sol url])                                                       | [Midterm I: 9:30AM - 10:45AM][week 06 game url]                              | [S1][week 06 game submit url S1], [S2][week 06 game submit url S2]         | --            |
| Week 7 ([2/22][recording 0222 url]), [2/24][recording 0224 url], [2/26][recording 0226 url])| [Sequential Logic: Clock, Latches, and Flip-Flops][week 07 url]              | [Week 07][read 07 url]                                                     | 2/28, 11:59PM |
| Week 8 ([3/1][recording 0301 url], 3/3, 3/5)                                                | [Sequential Logic: Finite State Machines][week 08 url]                       | Week 08                                                                    | 3/7, 11:59PM  |
| Week 9 (3/8, 3/10, 3/12)                                                                    | Sequential Logic: Registers, Counters, Shifters, and Arithmetic              | Week 09                                                                    | 3/14, 11:59PM |
| Spring Recess (Mar 15  - Mar 19)                                                            | --                                                                           | --                                                                         | --            |
| Week 10 (3/22)                                                                              | Practice Midterm II                                                          | --                                                                         | --            |
| Week 10 (3/24)                                                                              | Midterm II: 9:30AM - 10:45AM                                                 | --                                                                         | --            |
| Week 11 (3/29, 3/31)                                                                        | Register-Transfer Level Design                                               | Week 11                                                                    | 4/4, 11:59PM  |
| Week 12 (4/5, 4/7, 4/9)                                                                     | Register Memory Components and FIFO                                          | Week 12                                                                    | 4/11, 11:59PM |
| Week 13 (4/12, 4/14, 4/16)                                                                  | Optimizations and Tradeoffs                                                  | Week 13                                                                    | 4/18, 11:59PM |
| Week 14 (4/19, 4/21, 4/23)                                                                  | Physical Implementation on ICs                                               | Week 14                                                                    | 4/25, 11:59PM |
| Week 15 (4/26, 4/28, 4/30)                                                                  | Programmable Processors                                                      | Week 15                                                                    | 5/02, 11:59PM |
| Week 16 (5/3, 5/5)                                                                          | Class Review                                                                 | --                                                                         | --            |
| Study Days (5/7,5/8)                                                                        | --                                                                           | --                                                                         | --            |
| Week 17 (5/14)                                                                              | Final: 9:45AM - 11:45AM                                                      | --                                                                         | --            |

## Laboratory
| TIME                    | Topic                                        | Submissions                |                            | DEADLINE      |
| ---                     | ---                                          | ---                        | ---                        | ---           |
| Week 1 (1/12)           | --                                           | Section 1                  | Section 2                  | ---           |
| Week 2 (1/19)           | [Vivado Tutorial][lab 01 url]                | [Lab 01][labS1 01 sub url] | [Lab 01][labS2 01 sub url] | 1/24, 11:59PM |
| Week 3 (1/26)           | [Modeling Concepts][lab 02 url]              | [Lab 02][labS1 02 sub url] | [Lab 02][labS2 02 sub url] | 1/31, 11:59PM |
| Week 4 (2/2)            | [Numbering Systems][lab 03 url]              | [Lab 03][labS1 03 sub url] | [Lab 03][labS2 03 sub url] | 2/7, 11:59PM  |
| Week 5 (2/9)            | [Multi-Output Circuits][lab 04 url]          | [Lab 04][labS1 04 sub url] | [Lab 04][labS2 04 sub url] | 2/21, 11:59PM |
| Week 6 (2/16)           | --                                           | ---                        | ---                        | ---           |
| Week 7 (2/23)           | [Tasks Functions, and Testbench][lab 05 url] | [Lab 05][labS1 05 sub url] | [Lab 05][labS1 05 sub url] | 2/28, 11:59PM |
| Week 8 (3/2)            | [Modeling Latches and Flip-Flops][lab 06 url]| [Lab 06][labS1 06 sub url] | [Lab 06][labS2 06 sub url] | 3/7, 11:59PM  |
| Week 9 (3/9)            | Finite State Machines                        | [Lab 07][labS1 07 sub url] | [Lab 07][labS2 07 sub url] | 3/14, 11:59PM |
| Spring Recess (3/16)    | --                                           | ---                        | ---                        | ---           |
| Week 10 (3/23)          | --                                           | ---                        | ---                        | ---           |
| Week 11 (3/30)          | Modeling Registers and Counters              | Lab 08                     | Lab 08                     | 4/4, 11:59PM  |
| Week 12 (4/6)           | Architectural Wizard and IP Catalog          | Lab 09                     | Lab 09                     | 4/10, 11:59PM |
| Week 13 (4/13)          | Behavioral Modeling and Timing Constraints   | Lab 10                     | Lab 10                     | 4/18, 11:59PM |
| Week 14 (4/20)          | Sequential System Design using ASM Charts    | Lab 11                     | Lab 11                     | 4/25, 11:59PM |
| Week 15 (4/27)          | Catch-up Lab                                 | ---                        | ---                        | 5/2, 11:59PM  |
| Week 16 (4/4)           | --                                           | ---                        | ---                        | ---           |
| Study Days (May 07, 08) | --                                           | ---                        | ---                        | ---           |
| Week 17 (May 10)        | --                                           | ---                        | ---                        | ---           |

***
# Resources
## [Xilinx Vivado](https://www.xilinx.com/products/design-tools/vivado/vivado-webpack.html).
  - Installation
    - PC (Windows and Linux systems): [installation guide][xilinx vivado installation guide video url]
    - Mac (MacOS): requires a Linux virtual instance 
      - [Oracle VM VirtualBox (local, free)](https://www.virtualbox.org/): [installation guide][virtualbox guide url]
      - [Amazon Workspaces (cloud, paid)](https://aws.amazon.com/workspaces/): [installation guide][amazon workspace guide url]
  - [Xilinx Vivado Getting Started][xilinx vivado getting started url]

## [Basys 3 FPGA Trainer Board](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
  - Acquire
    - Pick up: Holme Hall 488, 1/13, 2:00pm-3:00pm.
    - Buy: [Digilent](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/).
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
[week 02 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_02_slides.pdf
[week 03 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_03_slides.pdf
[week 04 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_04_slides.pdf
[week 05 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_05_slides.pdf
[week 06 practice url]:../../../docs/exams/course_ee260_2021_spring/miterm_01/practice/
[week 06 practice submit url S1]:https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/Mjc0NjIyMTg2MTQ2/details
[week 06 practice submit url S2]:https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/Mjc0NjIyMTg2MTc5/details
[week 06 game url]:../../../docs/exams/course_ee260_2021_spring/miterm_01/game/
[week 06 sol url]:../../../docs/exams/course_ee260_2021_spring/miterm_01/solution/
[week 06 game submit url S1]:https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/Mjc2Mjc3MTc2OTM2/details
[week 06 game submit url S2]:https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/Mjc2Mjc3MTc2OTYy/details
[week 07 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_07_slides.pdf
[week 08 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_08_slides.pdf
[week 09 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_09_slides.pdf
[week 10 url]: https://classroom.github.com/a/jruqU2Sl
[week 11 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_11_slides.pdf
[week 12 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_12_slides.pdf
[week 13 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_13_slides.pdf
[week 14 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_14_slides.pdf
[week 15 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/slides/ee260_2021_spring_materials_week_15_slides.pdf
[week 16 url]: https://classroom.github.com/a/eqfZxWdk
[week 17 url]: https://classroom.github.com/a/ahPU1u-k

[recording urls]: # (recording urls)
[recording 0113 url]: https://youtu.be/RtppPuw2Thw
[recording 0115 url]: https://youtu.be/Io-uqv-oNEM
[recording 0120 url]: https://youtu.be/nSlZ9HoWbqk
[recording 0122 url]: https://youtu.be/WLKV46bScUY
[recording 0125 url]: https://youtu.be/zd7QDoAOB5M
[recording 0127 url]: https://youtu.be/qOvsE0DwB6g
[recording 0129 url]: https://youtu.be/GnCvNdikZ9E
[recording 0201 url]: https://youtu.be/aKAWfHtch7E
[recording 0203 url]: https://youtu.be/3XZm8G8HvGQ
[recording 0205 url]: https://youtu.be/TT6feNwPG5o
[recording 0208 url]: https://youtu.be/j1XKgbZsiyQ
[recording 0210 url]: https://youtu.be/tzZee1WCJjY
[recording 0212 url]: https://youtu.be/8y-eXbUz4pM
[recording 0217 url]: https://youtu.be/pNOfUSQwvdQ
[recording 0222 url]: https://youtu.be/Iy2d9AWodQk
[recording 0224 url]: https://youtu.be/LS11RUABmFo
[recording 0226 url]: https://youtu.be/OyeArTPWShU
[recording 0301 url]: https://youtu.be/anNbjOznNO8

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

[labs urls]: # (labs urls)
[lab 01 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_01.zip
[lab 02 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_02.zip
[lab 03 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_03.zip
[lab 04 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_04.zip
[lab 05 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_05.zip
[lab 06 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_06.zip

[labsS1 sub urls]: # (labs sub urls)
[labS1 01 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjUxODAxMjY0OTY2/details
[labS1 02 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjYwNDg4Mzk4MDg0/details
[labS1 03 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjY1MzY4MzI0NDg0/details
[labS1 04 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjcwMzc4NDI1ODY1/details
[labS1 05 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/Mjc3NjU2MDM3OTY2/details
[labS1 06 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjkxNDIzNDYxMzY2/details
[labS1 07 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MjkwOTk3NDQ5OTcz/details
[labS1 08 sub url]: # (labs sub urls)
[labS1 09 sub url]: # (labs sub urls)

[labsS2 sub urls]: # (labs sub urls)
[labS2 01 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/MjUxODI5NjI2OTgx/details
[labS2 02 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/MjYwNDg4Mzk4OTgy/details
[labS2 03 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/MjY1Njc3Mjk4Mjkz/details
[labS2 04 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/MjcwMzc4NDI2MDgy/details
[labS2 05 sub url]: https://classroom.google.com/u/0/w/MjUwMzMyNjE4MjA5/tc/Mjc2OTc0MjM5OTgx
[labS2 06 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/MjkxNjQ4MzQ4ODM3/details
[labS2 07 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MjA5/a/Mjk0Mjg5MTg0MzI5/details
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
