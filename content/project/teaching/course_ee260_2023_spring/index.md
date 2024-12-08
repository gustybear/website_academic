---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "EE260: Introduction to Digital Design"

subtitle: "Spring, 2023"

summary: "EE260 is the introductory course on digital circuit synthesis, focusing on the design and implementation of combinational logic, sequential logic, and basic central processor (van Neumann/Princeton architecture) through Verilog HDL and FPGA."

date: 2023-01-09T02:58:53+00:00
lastmod: 2023-01-09T02:58:53+00:00
featured: false
draft: false

authors:
- Yao Zheng
- Denny Landika
- John Taylor
- Anthony A. Apilado

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
- name: CRN
  url: ./project/teaching/course_ee260_2023_spring/#logistics
- name: Textbook
  url: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023
#- name: Sample lecture
#  url: https://youtu.be/3XZm8G8HvGQ
#- name: Sample laboratory
#  url: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_03.zip
#- name: Sample exam
#  url: ./docs/exams/course_ee260_2021_spring/final/practice/
---
***
# Executive Summary
This course explores the foundation of digital circuit design, starting from Boolean algebra, through combinational and sequential logic, to finite state machines and basic central processing units (CPUs) under von Neumann architecture. The associated laboratory segment introduces modern digital design techniques, e.g., hardware description language ([Verilog] HDL) and field-programmable gate array (FPGA), to model, implement, and test the aforementioned digital circuits.
***

# Logistics {#logistics}
- **CRN**
| EE260 001 | EE260 002 |
| ---   | ---   |
| 87422 | 87423 |

- **Personnel**
|                                                       |                                             |
| ----                                                  | ---                                         |
| Lecturer: [Yao Zheng](mailto:yao.zheng@hawaii.edu)    | Office Hours: see [here](../../../#contact) |
| TA: [Denny Landika](mailto:dennyvp@hawaii.edu)        | Session 1, Office Hours: HH451, F 12:00pm - 1:00pm                |
| TA: [Ryan Taylar](mailto:jrtaylor@hawaii.edu)         | Session 2, Office Hours: HH451, T 4:16pm - 5:16pm                 |
| Grader: [Anthony Apilado](mailto:apiladoa@hawaii.edu) | --                                          |

- **Classroom**
| Time               | Location           | Textbook/HW                                                                                          | HW/Exam Effort |
| ----               | ---                | ---                                                                                                  | ---            |
| MWF 9:30am-10:20am | Art Building 101   | [EE260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023) | Individual     |

- **Laboratory**
| Session | Time             | Location         | Report Effort |
| ---     | ----             | ---              | ---           |
| 01      | T 9:00am-11:45am | Holmes Hall 451  |  Group        |
| 02      | T 1:30pm-4:15pm  | Holmes Hall 451  |  Group        |

***
# Grading

- **Breakdown**
| Participation | Challenge | Labs           | Midterms (2) | Final |
| ----------    | ------    | -------------- | -------      | ---   |
| 5%            | 20%       | 25%            | 30%          | 20%   |

- **Curves**
| Linear                         | Bell            |
| ---                            | ---             |
| participation, challenge, labs | Midterms, Final |

- **Cutoffs**
| A-     | B-    | C-    |
| ------ | ----- | ----- |
| 70%    | 50%   | 30%   |

- **Proscribed Conduct**: Copying or otherwise cheating on homework, lab reports, or exam will result in a failing grade for the course. More details can be found at student conduct code policies, [III.C.](http://studentaffairs.manoa.hawaii.edu/policies/conduct_code/proscribed_conduct.php)

***
# Schedule
## Lecture
| TIME                         | TOPICS                                                                 | READING/HW/EXAM              | DEADLINE      |
| ---                          | ---                                                                    | ---                          | ---           |
| Week 1 (1/9, 1/11, 1/13)     | [Course Logistic and Introduction][week 01 url]                        | [Read/HW 01][read 01 url]    | 1/15, 11:59PM |
| Week 2 (1/18 1/20)           | [Number Systems][week 02 url]                                          | [Read/HW 02][read 02 url]    | 1/22, 11:59PM |
| Week 3 (1/23, 1/25, 1/27)    | [Combinational Logic: Switches, Transistors, Logic Gates][week 03 url] | [Read/HW 03][read 03 url]    | 1/29, 11:59PM |
| Week 4 (1/30, 2/1, 2/3)      | [Combinational Logic: Boolean Algebra][week 04 url]                    | [Read/HW 04][read 04 url]    | 2/5, 11:59PM  |
| Week 5 (2/6, 2/8, 2/10)      | [Combinational Logic: Design Process, More Gates][week 05 url]         | [Read/HW 05][read 05 url]    | 2/12, 11:59PM |
| Week 6 (2/13)                | Practice Midterm I                                                     | --                           | --            |
| Week 6 (2/15)                | Midterm I: 9:30AM - 10:20AM                                            | --                           | --            |
| Week 6/7 (2/17, 2/22, 2/24)  | [Sequential Logic: Clock, Latches, and Flip-Flops][week 07 url]        | [Read/HW 07][read 07 url]    | 2/26, 11:59PM |
| Week 8 (2/27, 3/1, 3/3)      | [Sequential Logic: Finite State Machines][week 08 url]                 | [Read/HW 08][read 08 url]    | 3/5, 11:59PM  |
| Week 9 (3/6, 3/8, 3/10)      | [Sequential Logic: Registers, Counters, Shifters, and Arithmetic][week 09 url]  | [Read/HW 09][read 09 url]                   | 3/12, 11:59PM |
| Spring Recess (3/13  - 3/17) | --                                                                     | --                           | --            |
| Week 10 (3/20)               | Practice Midterm II                                                    | --                           | --            |
| Week 10 (3/22)               | Midterm II: 9:30AM - 10:20AM                                           | --                           | --            |
| Week 10/11 (3/24, 3/29, 3/31)| [Register-Transfer Level Design][week 11 url]                          | [Read/HW 11][read 11 url]    | 4/2, 11:59PM  |
| Week 12 (4/3, 4/5)           | [Register Memory Components and FIFO][week 12 url]                     | [Read/HW 12][read 12 url]    | 4/9, 11:59PM  |
| Week 13 (4/10, 4/12, 4/14)   | [Optimizations and Tradeoffs][week 13 url]                             | [Read/HW 13][read 13 url]    | 4/16, 11:59PM |
| Week 14 (4/17, 4/19, 4/21)   | [Physical Implementation on ICs][week 14 url]                          | [Read/HW 14][read 14 url]    | 4/23, 11:59PM |
| Week 15 (4/24, 4/26, 4/28)   | [Programmable Processors][week 15 url]                                 | [Read/HW 15][read 15 url]    | 4/30, 11:59PM |
| Week 16 (5/1, 5/3)           | Review, Practice Final                                                 | --                           | --            |
| Study Days (4/5)             | --                                                                     | --                           | --            |
| Week 17 (5/12)               | Final: 9:45AM - 11:45AM                                                | --                           | 5/12, 11:45AM |

## Laboratory
| TIME                                 | Materials                                         | Virtual               | DEADLINE                      |
| ---                                  | ---                                               | ---                   | ---                           |
| Week 1 (1/10)                        | --                                                | ---                   | ---                           |
| Week 2 (1/17)                        | [Vivado Tutorial][lab 01 url]                     | [Vlab 01][vlab01 url] | 1/24, BOS                     |
| Week 3 (1/24)                        | [Modeling Concepts][lab 02 url]                   | [Vlab 02][vlab02 url] |  1/31, BOS                    |
| Week 4 (1/31)                        | [Numbering Systems][lab 03 url]                   | [Vlab 03][vlab03 url] |  2/7, BOS                     |
| Week 5 (2/7)                         | [Multi-Output Circuits][lab 04 url]               | [Vlab 04][vlab04 url] |  2/14, BOS                    |
| Week 6 (2/14)                        | --                                                |  --                   |  --                           |
| Week 7 (2/21)                        | [Tasks Functions, and Testbench][lab 05 url]      | [Vlab 05][vlab05 url] |  2/28, BOS                    |
| Week 8 (2/28)                        | [Modeling Latches and Flip-Flops][lab 06 url]     | [Vlab 06][vlab06 url] |  3/7, BOS                     |
| Week 9 (3/7)                         | [Finite State Machines][lab 07 url]               |  Vlab 07              |  3/28, BOS                    |
| Spring Recess (3/15)                 | --                                                |  --                   |  --                           |
| Week 10 (3/21)                       | --                                                |  --                   |  --                           |
| Week 11 (3/28)                       | [Modeling Registers and Counters][lab 08 url]     |  Vlab 08              |  4/4, BOS                     |
| Week 12 (4/4)                        | [Architectural Wizard and IP Catalog][lab 09 url] |  Vlab 09              |  4/11, BOS                    |
| Week 13 (4/11)                       | [Behavioral Modeling and Timing Constraints][lab 10 url] |  Vlab 10              | 4/18, BOS              |
| Week 14 (4/18)                       | [Sequential System Design using ASM Charts][lab 11 url]  |  Vlab 11              | 4/25, BOS              |
| Week 15 (4/25)                       | Catch-up Lab (if needed)                          |  --                   |                               |
| Week 16 (5/2)                        | --                                                |  --                   | --                            |
| Week 17 (5/10)                       | --                                                |  --                   | --                            |

***
# Resources
## [Xilinx Vivado Design Suite - HLx Edition: Update 2 - 2018.2](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vivado-design-tools/archive.html).
  - Access
    - Holmes Hall 387: M-F 7:30am-5:30pm
  - Installation
    - PC ([Windows](https://www.xilinx.com/member/forms/download/xef-vivado.html?filename=Xilinx_Vivado_SDK_Web_2018.2_0614_1954_Win64.exe) and [Linux](https://www.xilinx.com/member/forms/download/xef-vivado.html?filename=Xilinx_Vivado_SDK_Web_2018.2_0614_1954_Lin64.bin) systems): [installation guide][xilinx vivado installation guide video url]
    - Mac (MacOS): requires a Linux virtual instance 
      - [Multipass](https://multipass.run)
      - [Amazon Workspaces (cloud, paid)](https://aws.amazon.com/workspaces/)
  - [Xilinx Vivado Getting Started][xilinx vivado getting started url]

## [Basys 3 FPGA Trainer Board](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
  - Acquire
    - In-House: Holme Hall 451, during lab sessions.
    - Buy: [Digilent](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/).
  - [Basys3 Master XDC File][basys3 master xdc file url]
  - [Basys3 Reference Manual][basys3 reference manual url]
  - [Basys3 Schematic][basys3 schematic url]

### Verilog
- [Introduction to Verilog][introduction to verilog url]
- [Introduction to Verilog Video][introduction to verilog video url]
- [Verilog Short Reference](https://web.stanford.edu/class/ee183/handouts_win2003/VerilogQuickRef.pdf)
- [Verilog Full Reference](https://sutherland-hdl.com/pdfs/verilog_2001_ref_guide.pdf)


[week urls]: # (week urls)
[week 01 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_01_slides.pdf
[week 02 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_02_slides.pdf
[week 03 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_03_slides.pdf
[week 04 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_04_slides.pdf
[week 05 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_05_slides.pdf
[week 06 practice url]:../../../docs/exams/course_ee260_2023_spring/miterm_01_practice/
[week 06 practice submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDY4ODg0Njc1NjU2/details
[week 06 practice submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDY5MTc5NjI0Mjk4/details
[week 06 game url]:../../../docs/exams/course_ee260_2023_spring/miterm_01_game/
[week 06 sol url]:../../../docs/exams/course_ee260_2023_spring/miterm_01_solution/
[week 06 game submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDcwMDE3NzQ5NTQ3/details
[week 06 game submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDcwMDE4MjM2ODIx/details
[week 07 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_07_slides.pdf
[week 08 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_08_slides.pdf
[week 09 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_09_slides.pdf
[week 10 practice url]:../../../docs/exams/course_ee260_2023_spring/miterm_02_practice/
[week 10 practice submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/MzUzNDE4MTU2MDk2/details
[week 10 practice submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/MzUzNDE4MTU2MjUw/details
[week 10 game url]:../../../docs/exams/course_ee260_2023_spring/miterm_02_game/
[week 10 sol url]:../../../docs/exams/course_ee260_2023_spring/miterm_02_solution/
[week 10 game submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/MzUzNDE4MTU2MTUz/details
[week 10 game submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/MzUzNDE4MTU2Mjc2/details
[week 11 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_11_slides.pdf
[week 12 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_12_slides.pdf
[week 13 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_13_slides.pdf
[week 14 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_14_slides.pdf
[week 15 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_15_slides.pdf
[week 16 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/slides/ee260_2023_spring_materials_week_16_slides.pdf
[week 16 practice url]:../../../docs/exams/course_ee260_2023_spring/final_practice/
[week 17 game url]:../../../docs/exams/course_ee260_2023_spring/final_game/
[week 17 game submit url S1]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NTEwNTEwNjIyMTA0/details
[week 17 game submit url S2]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NTEwNTEwNjYyMzc3/details

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
[recording 0303 url]: https://youtu.be/bKm5rYalXHA
[recording 0305 url]: https://youtu.be/_IhJ0ECNnSY
[recording 0308 url]: https://youtu.be/9vp-RKdkr5I
[recording 0310 url]: https://youtu.be/q2X74p8BGSY
[recording 0312 url]: https://youtu.be/VOkZueH-JeU
[recording 0322 url]: https://youtu.be/Ah44ermxwx8
[recording 0329 url]: https://youtu.be/J_4rpI6FpI0
[recording 0331 url]: https://youtu.be/tDa7I-SHRQE
[recording 0405 url]: https://youtu.be/kYcv13UohG8
[recording 0407 url]: https://youtu.be/frvdQcka0x0
[recording 0409 url]: https://youtu.be/Ad3YPhXkpvc
[recording 0412 url]: https://youtu.be/kcbqTWbn3wM
[recording 0414 url]: https://youtu.be/xhgT7T8U130
[recording 0416 url]: https://youtu.be/evFDDTSXZCo
[recording 0419 url]: https://youtu.be/4Fg3OoCjEho
[recording 0421 url]: https://youtu.be/zmqfPlbq4Ww
[recording 0423 url]: https://youtu.be/qz9bKvlZCJY
[recording 0426 url]: https://youtu.be/pX8NtuTNpvE
[recording 0428 url]: https://youtu.be/iV4xkz7ygaI
[recording 0430 url]: https://youtu.be/uaOPjOimqsg
[recording 0503 url]: https://youtu.be/HIHR0tBOeWw
[recording 0505 url]: https://youtu.be/PWIIeYGItZY

[read urls]: # (reading urls)
[read 01 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/1/section/1
[read 02 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/2/section/1
[read 03 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/3/section/1
[read 04 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/4/section/1
[read 05 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/5/section/1
[read 06 url]: # (reading urls)
[read 07 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/6/section/1
[read 08 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/7/section/1
[read 09 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/8/section/1
[read 10 url]: # (reading urls)
[read 11 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/9/section/1
[read 12 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/10/section/1
[read 13 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/11/section/1
[read 14 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/12/section/1
[read 15 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/13/section/1
[read 16 url]: # (reading urls)
[read 17 url]: # (reading urls)

[labs urls]: # (labs urls)
[lab 01 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_01.zip
[lab 02 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_02.zip
[lab 03 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_03.zip
[lab 04 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_04.zip
[lab 05 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_05.zip
[lab 06 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_06.zip
[lab 07 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_07.zip
[lab 08 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_08.zip
[lab 09 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_09.zip
[lab 10 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_10.zip
[lab 11 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2023_spring/labs/lab_11.zip

[vlabs urls]: # (vlabs urls)
[vlab01 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/14/section/1
[vlab02 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/14/section/2
[vlab03 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/14/section/3
[vlab04 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/14/section/4
[vlab05 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/14/section/5
[vlab06 url]: https://learn.zybooks.com/zybook/HAWAIIEE260Spring2023/chapter/14/section/6


[labsS1 sub urls]: # (labs sub urls)
[labS1 01 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDUyODk1NDIwNjQy/details
[labS1 02 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDYyNjIwOTA1ODkx/details
[labS1 03 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDY0MzQyNDQ1MjMz/details
[labS1 04 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDY2MjUzNjQxOTUz/details
[labS1 05 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDY2MjUzNjQxOTUz/details
[labS1 06 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDc0MDY1MzA2MzA2/details
[labS1 07 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDgwMzIwMDYyNjgy/details
[labS1 08 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDgwMzIwMDYyNjgy/details
[labS1 09 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDk4ODYzNDQ0NzA5/details
[labS1 10 sub url]: https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NTAwMjMzMjUzNDU0/details
[labS1 11 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MzE1NTAzODQ0MjE4/details


[labsS2 sub urls]: # (labs sub urls)
[labS2 01 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDUyOTMyNTMwMTM0/details
[labS2 02 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDYyNTMyNzU1NzEz/details
[labS2 03 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDY1NTMxMjYwMDEy/details
[labS2 04 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDY2MzY4ODIxMTk4/details
[labS2 05 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDc0Mjc1MTk4NDQx/details
[labS2 06 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDcxMDA0OTUxMDk4/details
[labS2 07 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDc4OTUxNDc1NzEy/details
[labS2 08 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDgzNzMzODc4ODUy/details
[labS2 09 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDk4OTA4MjM2ODc3/details
[labS2 10 sub url]: https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NTAwMjgwMTQ1MzE2/details
[labS2 11 sub url]: https://classroom.google.com/c/MjUwMzMyNjE4MTk4/a/MzE1NTAzODQ0MjE4/details

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

[introduction to verilog url]: https://athena.ecs.csus.edu/~arad/csc142/intro_verilog_hdl.pdf
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
