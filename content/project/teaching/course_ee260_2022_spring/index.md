---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "EE260: Introduction to Digital Design"

subtitle: "Spring, 2022 (Virtual -> In Person)"

summary: "EE260 is the introductory course on digital circuit synthesis, focusing on the design and implementation of combinational logic, sequential logic, and basic central processor (van Neumann/Princeton architecture) through Verilog HDL and FPGA."

date: 2022-01-08T10:51:00-10:00
lastmod: 2022-01-08T10:51:00-10:00
featured: false
draft: true

authors:
- Yao Zheng
- Jannatun Noor Sameera
- Md Sakib Galib Sourav
- Dylan Sodetani

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
#- current semester

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
  url: ./project/teaching/course_ee260_2022_spring/#logistics
- name: Textbook
  url: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022
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
| 80461 | 80462 |

- **Personnel**
|                                                         |                                             |
| ----                                                    | ---                                         |
| Lecturer: [Yao Zheng](mailto:yao.zheng@hawaii.edu)      | Office Hours: see [here](../../../#contact) |
| TA: [Md Sakib Galib Sourav](mailto:msgs@hawaii.edu)     | Session 01, Office Hours: T 11:45am-12:30pm |
| TA: [Jannatun Noor Sameera](mailto:jsameera@hawaii.edu) | Session 02, Office Hours: T 4:15pm-5:00pm   |
| Grader: [Dylan Sodetani](mailto:dylans88@hawaii.edu)    | --                                          |

- **Classroom**
| Time               | Location                                                                                                | Textbook/HW                                                                                          | Onine Exams      | In-Person Exams     | HW/Exam Effort |
| ----               | ---                                                                                                     | ---                                                                                                  | ---              | ---                 | ---            |
| MWF 9:30am-10:20am | [Zoom](https://hawaii.zoom.us/j/5764842348?pwd=cGdVMzBnOHlZbDkrNmErb0QxdTllUT09) -> Kuykendall Hall 305 | [EE260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022) | Google Classroom | Kuykendall Hall 305 | Individual     |

- **Laboratory**
| Session | Time             | Location                                                                                             | Report                                                                          | Report Effort |
| ---     | ----             | ---                                                                                                  | ---                                                                             | ---           |
| 01      | T 9:00am-11:45am | [Zoom](https://hawaii.zoom.us/j/96120437928?pwd=eXllYTdxdkNDTFRtYXNWSTlkNFphUT09) -> Holmes Hall 451 | [Google Classroom](https://classroom.google.com/c/NDUyODk1Mzg3MDc1?cjc=lcc4x2a) | Group         |
| 02      | T 1:30pm-4:15pm  | [Zoom](https://zoom.us/j/97952958777?pwd=MTJGN3pJaU8vNXkrYUJBTGpFb3JUQT09) -> Holmes Hall 451        | [Google Classroom](https://classroom.google.com/c/NDUyOTMyNTI5NzEz?cjc=jlop76l) | Group         |

***
# Grading

- **Breakdown**
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
| TIME                         | TOPICS                                                                 | READING/HW/EXAM              | DEADLINE      |
| ---                          | ---                                                                    | ---                          | ---           |
| Week 1 (1/10, 1/12, 1/14)    | [Course Logistic and Introduction][week 01 url]                        | [Read/HW 01][read 01 url]    | 1/18, 11:59PM |
| Week 2 (1/19 1/21)           | [Number Systems][week 02 url]                                          | [Read/HW 02][read 02 url]    | 1/23, 11:59PM |
| Week 3 (1/24, 1/26, 1/28)    | [Combinational Logic: Switches, Transistors, Logic Gates][week 03 url] | [Read/HW 03][read 03 url]    | 1/30, 11:59PM |
| Week 4 (1/31, 2/2, 2/4)      | [Combinational Logic: Boolean Algebra][week 04 url]                    | [Read/HW 04][read 04 url]    | 2/6, 11:59PM  |
| Week 5 (2/7, 2/9, 2/11)      | [Combinational Logic: Design Process, More Gates][week 05 url]         | [Read/HW 05][read 05 url]    | 2/13, 11:59PM |
| Week 6 (2/14)                | [Practice Midterm I][week 06 practice url]                             | [PMT 01,Sec 01][week 06 practice submit url S1]; [PMT 01,Sec 02][week 06 practice submit url S2] | --            |
| Week 6 ([2/16][week 06 sol url]) | [Midterm I: 9:30AM - 10:45AM][week 06 game url]                        | [MT 01,Sec 01][week 06 game submit url S1]; [MT 01,Sec 02][week 06 game submit url S2]   | --            |
| Week 6/7 (2/18, 2/23, 2/25)  | [Sequential Logic: Clock, Latches, and Flip-Flops][week 07 url]        | [Read/HW 07][read 07 url]    | 2/27, 11:59PM |
| Week 8 (2/28, 3/2, 3/4)      | [Sequential Logic: Finite State Machines][week 08 url]                 | [Read/HW 08][read 08 url]    | 3/6, 11:59PM  |
| Week 9 (3/7, 3/9, 3/11)      | [Sequential Logic: Registers, Counters, Shifters, and Arithmetic][week 09 url]  | [Read/HW 09][read 09 url]                   | 3/27, 11:59PM |
| Spring Recess (3/14  - 3/18) | --                                                                     | --                           | --            |
| Week 10 (3/21)               | [Practice Midterm II][week 10 practice url]                            | [PMT 02,Sec 01][week 10 practice submit url S1]; [PMT 02,Sec 02][week 10 practice submit url S2] | --            |
| Week 10 (3/23)               | [Midterm II: 9:30AM - 10:45AM][week 10 game url]                       | [MT 02,Sec 01][week 10 game submit url S1]; [MT 02,Sec 02][week 10 game submit url S2]   | --            |
| Week 11 (3/28, 3/30, 4/1)    | [Register-Transfer Level Design][week 11 url]                          | [Read/HW 11][read 11 url]    | 4/3, 11:59PM  |
| Week 12 (4/4, 4/6, 4/8)      | [Register Memory Components and FIFO][week 12 url]                     | [Read/HW 12][read 12 url]    | 4/10, 11:59PM |
| Week 13 (4/11, 4/13)         | [Optimizations and Tradeoffs][week 13 url]                             | [Read/HW 13][read 13 url]    | 4/17, 11:59PM |
| Week 14 (4/18, 4/20, 4/22)   | [Physical Implementation on ICs][week 14 url]                          | [Read/HW 14][read 14 url]    | 4/24, 11:59PM |
| Week 15 (4/25, 4/27, 4/29)   | [Programmable Processors][week 15 url]                                 | [Read/HW 15][read 15 url]    | 5/1, 11:59PM  |
| Week 16 (5/2, 5/4)           | [Review][week 16 url], [Practice Final][week 16 practice url]          | All remaining Read/HW (50\%) | 5/8, 11:59PM  |
| Study Days (5/6)             | --                                                                     | --                           | --            |
| Week 17 (5/9)                | [Final: 9:45AM - 11:45AM][week 17 game url]                            | [FE,Sec 01][week 17 game submit url S1]; [FE,Sec 02][week 17 game submit url S2]         | 5/9, 11:45AM  |

## Laboratory
| TIME                                 | TOPICS                                            | REPORT                                                                 | DEADLINE                      |
| ---                                  | ---                                               | ---                                                                    | ---                           |
| Week 1 (1/11)                        | --                                                | --                                                                     | ---                           |
| Week 2 ([1/20][recording 0115 url])  | [Vivado Tutorial][lab 01 url]                     | [Rpt 01, Sec 01][labS1 01 sub url]; [Rpt 01, Sec 02][labS2 01 sub url] | ~~1/23~~ ~~1/25~~ 3/1, 8:00AM |
| Week 3 ([1/25][recording 0125 url])  | [Modeling Concepts][lab 02 url]                   | [Rpt 02, Sec 01][labS1 02 sub url]; [Rpt 02, Sec 02][labS2 02 sub url] | ~~2/1~~ 3/1, 8:00AM           |
| Week 4 ([2/1][recording 0201 url])   | [Numbering Systems][lab 03 url]                   | [Rpt 03, Sec 01][labS1 03 sub url]; [Rpt 03, Sec 02][labS2 03 sub url] | ~~2/8~~ 3/1, 8:00AM           |
| Week 5 ([2/8][recording 0208 url])   | [Multi-Output Circuits][lab 04 url]               | [Rpt 04, Sec 01][labS1 04 sub url]; [Rpt 04, Sec 02][labS2 04 sub url] | ~~2/22~~ 3/1, 8:00AM          |
| Week 6 (2/15)                        | --                                                | ---          ---                                                       | ---                           |
| Week 7 ([2/22][recording 0222 url])  | [Tasks Functions, and Testbench][lab 05 url]      | [Rpt 05, Sec 01][labS1 05 sub url]; [Rpt 05, Sec 02][labS2 05 sub url] | 3/1, 8:00AM                   |
| Week 8 ([3/1][recording 0301 url])   | [Modeling Latches and Flip-Flops][lab 06 url]     | [Rpt 06, Sec 01][labS1 06 sub url]; [Rpt 06, Sec 02][labS2 06 sub url] | 3/8, 8:00AM                   |
| Week 9 ([3/8][recording 0308 url])   | [Finite State Machines][lab 07 url]               | [Rpt 07, Sec 01][labS1 07 sub url]; [Rpt 07, Sec 02][labS2 07 sub url] | 3/29, 8:00AM                  |
| Spring Recess (3/15)                 | --                                                | ---          ---                                                       | ---                           |
| Week 10 (3/22)                       | --                                                | ---          ---                                                       | ---                           |
| Week 11 ([3/29][recording 0329 url]) | [Modeling Registers and Counters][lab 08 url]     | [Rpt 08, Sec 01][labS1 08 sub url]; [Rpt 08, Sec 02][labS2 08 sub url] | 4/5, 8:00AM                   |
| Week 12 ([4/5][recording 0405 url])  | [Architectural Wizard and IP Catalog][lab 09 url] | [Rpt 09, Sec 01][labS1 09 sub url]; [Rpt 09, Sec 02][labS2 09 sub url] | 4/12( 5/3 for section 2), 8:00AM                  |
| Week 13 ([4/12][recording 0412 url], [Set input delay](https://www.xilinx.com/video/hardware/setting-input-delay.html), [Set output delay](https://www.xilinx.com/video/hardware/setting-output-delay.html) | [Behavioral Modeling and Timing Constraints][lab 10 url]    | [Rpt 10, Sec 01][labS1 10 sub url]; [Rpt 10, Sec 02][labS2 10 sub url] | 4/19, 8:00AM                  |
| Week 14 ([4/19][recording 0419 url]) | [Sequential System Design using ASM Charts][lab 11 url]         | Rpt 11, Sec 01; Rpt 11, Sec 02                                         | 4/26, 8:00AM                  |
| Week 15 (4/26)                       | Catch-up Lab                                      | ---          ---                                                       | 5/3, 8:00AM                   |
| Week 16 (5/3)                        | --                                                | ---          ---                                                       | ---                           |
| Study Days (5/7)                     | --                                                | ---          ---                                                       | ---                           |
| Week 17 (5/10)                       | --                                                | ---          ---                                                       | ---                           |

***
# Resources
## [Xilinx Vivado Design Suite - HLx Edition: Update 2 - 2018.2](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vivado-design-tools/archive.html).
  - Installation
    - PC ([Windows](https://www.xilinx.com/member/forms/download/xef-vivado.html?filename=Xilinx_Vivado_SDK_Web_2018.2_0614_1954_Win64.exe) and [Linux](https://www.xilinx.com/member/forms/download/xef-vivado.html?filename=Xilinx_Vivado_SDK_Web_2018.2_0614_1954_Lin64.bin) systems): [installation guide][xilinx vivado installation guide video url]
    - Mac (MacOS): requires a Linux virtual instance 
      - [Oracle VM VirtualBox (local, free)](https://www.virtualbox.org/): [installation guide][virtualbox guide url]
      - [Amazon Workspaces (cloud, paid)](https://aws.amazon.com/workspaces/): [installation guide][amazon workspace guide url]
  - [Xilinx Vivado Getting Started][xilinx vivado getting started url]

## [Basys 3 FPGA Trainer Board](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
  - Acquire
    - In-House: Holme Hall 305, during lab sessions.
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
[week 01 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_01_slides.pdf
[week 02 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_02_slides.pdf
[week 03 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_03_slides.pdf
[week 04 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_04_slides.pdf
[week 05 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_05_slides.pdf
[week 06 practice url]:../../../docs/exams/course_ee260_2022_spring/miterm_01_practice/
[week 06 practice submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDY4ODg0Njc1NjU2/details
[week 06 practice submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDY5MTc5NjI0Mjk4/details
[week 06 game url]:../../../docs/exams/course_ee260_2022_spring/miterm_01_game/
[week 06 sol url]:../../../docs/exams/course_ee260_2022_spring/miterm_01_solution/
[week 06 game submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/NDcwMDE3NzQ5NTQ3/details
[week 06 game submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/NDcwMDE4MjM2ODIx/details
[week 07 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_07_slides.pdf
[week 08 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_08_slides.pdf
[week 09 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_09_slides.pdf
[week 10 practice url]:../../../docs/exams/course_ee260_2022_spring/miterm_02_practice/
[week 10 practice submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/MzUzNDE4MTU2MDk2/details
[week 10 practice submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/MzUzNDE4MTU2MjUw/details
[week 10 game url]:../../../docs/exams/course_ee260_2022_spring/miterm_02_game/
[week 10 sol url]:../../../docs/exams/course_ee260_2022_spring/miterm_02_solution/
[week 10 game submit url S1]:https://classroom.google.com/c/NDUyODk1Mzg3MDc1/a/MzUzNDE4MTU2MTUz/details
[week 10 game submit url S2]:https://classroom.google.com/c/NDUyOTMyNTI5NzEz/a/MzUzNDE4MTU2Mjc2/details
[week 11 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_11_slides.pdf
[week 12 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_12_slides.pdf
[week 13 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_13_slides.pdf
[week 14 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_14_slides.pdf
[week 15 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_15_slides.pdf
[week 16 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/slides/ee260_2022_spring_materials_week_16_slides.pdf
[week 16 practice url]:../../../docs/exams/course_ee260_2022_spring/final_practice/
[week 17 game url]:../../../docs/exams/course_ee260_2022_spring/final_game/
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
[read 01 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/1/section/1
[read 02 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/2/section/1
[read 03 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/3/section/1
[read 04 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/4/section/1
[read 05 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/5/section/1
[read 06 url]: # (reading urls)
[read 07 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/6/section/1
[read 08 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/7/section/1
[read 09 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/8/section/1
[read 10 url]: # (reading urls)
[read 11 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/9/section/1
[read 12 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/10/section/1
[read 13 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/11/section/1
[read 14 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/12/section/1
[read 15 url]: https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2022/chapter/13/section/1
[read 16 url]: # (reading urls)
[read 17 url]: # (reading urls)

[labs urls]: # (labs urls)
[lab 01 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_01.zip
[lab 02 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_02.zip
[lab 03 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_03.zip
[lab 04 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_04.zip
[lab 05 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_05.zip
[lab 06 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_06.zip
[lab 07 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_07.zip
[lab 08 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_08.zip
[lab 09 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_09.zip
[lab 10 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_10.zip
[lab 11 url]: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2022_spring/labs/lab_11.zip


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
