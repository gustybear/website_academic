---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "EE361: Digital Systems & Computer Design"

subtitle: "Fall, 2023"

summary: "Design methodology, processor design, control design, memory organization, system organization. Pre: 205 and 260, or consent."

date: 2023-01-09T02:58:53+00:00
lastmod: 2023-01-09T02:58:53+00:00
featured: false
draft: true

authors:
- Yao Zheng
- Denny Landika

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
  url: ./project/teaching/course_ee361_2023_spring/#logistics
- name: Textbook
  url: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023
#- name: Sample lecture
#  url: https://youtu.be/3XZm8G8HvGQ
#- name: Sample laboratory
#  url: https://gustybear-websites.s3-us-west-2.amazonaws.com/course_ee260_2021_spring/labs/lab_03.zip
#- name: Sample exam
#  url: ./docs/exams/course_ee260_2021_spring/final/practice/
---
***
# Executive Summary
***Design methodology, processor design, control design, memory organization, system organization. Pre: 205 and 260, or consent.***

# Logistics {#logistics}
- **CRN**
| EE260 001 | 
| ---       | 
| 70527     | 

- **Personnel**
|                                                       |                                             |
| ----                                                  | ---                                         |
| Lecturer: [Yao Zheng](mailto:yao.zheng@hawaii.edu)    | Office Hours: see [here](../../../#contact) |
| TA: [Denny Landika](mailto:dennyvp@hawaii.edu)        |                                             |

- **Classroom**
| Time               | Location        | Textbook/HW                                                                                          | HW/Exam Effort |
| ----               | ---             | ---                                                                                                  | ---            |
| MWF 9:30am-10:20am | HIG110          | [EE361: Digital Systems & Computer Design](https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023) | Individual     |

- **Laboratory**
| Session | Time             | Location         | Report Effort |
| ---     | ----             | ---              | ---           |
| 01      | T 9:00am-11:45am | Holmes Hall 451  | Group         |
| 02      | T 1:30pm-4:15pm  | Holmes Hall 451  | Group         |

***
# Grading
<!-- NOT DONE YET -->
- **Breakdown**
| Participation | Challenge | Labs           | Midterms (2) | Final |
| ----------    | ------    | -------------- | -------      | ---   |
| 5%            | 20%       | 25%            | 30%          | 20%   |

- **Curves**
| Linear                                   | Bell            |
| ---                                      | ---             |
| participation, quizzes, labs, homework   | Midterms, Final |

- **Cutoffs**
| A-     | B-    | C-    |
| ------ | ----- | ----- |
| 90%    | 80%   | 70%   |

- **Proscribed Conduct**: Copying or otherwise cheating on homework, lab reports, or exam will result in a failing grade for the course. More details can be found at student conduct code policies, [III.C.](http://studentaffairs.manoa.hawaii.edu/policies/conduct_code/proscribed_conduct.php)

***
# Schedule
## Lecture
| TIME                          | TOPICS                                    | READING/HW                | DEADLINE       |
|-------------------------------|-------------------------------------------|---------------------------|----------------|
| Week 1 (8/21, 8/23, 8/25)     | [Introduction][week 01 url]               | [Read/HW 01][read 01 url] | 8/27, 11:59PM  |
| Week 2 (8/28, 8/30, 9/1)      | [Computer Abstract][week 02 url]          | [Read/HW 02][read 02 url] | 9/3, 11:59PM   |
| Week 3 (9/6, 9/8)             | [Computer Tech][week 03 url]              | [Read/HW 03][read 03 url] | 9/10, 11:59PM  |
| Week 4 (9/11, 9/13, 9/15)     | [Instructions: Part 1][week 04 url]       | [Read/HW 04][read 04 url] | 9/17, 11:59PM  |
| Week 5 (9/18, 9/20, 9/22)     | [Instructions: Part 2][week 05 url]       | [Read/HW 05][read 05 url] | 9/24, 11:59PM  |
| Week 6 (9/25, 9/27, 9/29)     | [Instructions: Part 3][week 06 url]       | [Read/HW 06][read 06 url] | 10/1, 11:59PM  |
| Week 7 (10/2, 10/4, 10/6)     | [Arithmetic: Part 1][week 07 url]         | [Read/HW 07][read 07 url] | 10/8, 11:59PM  |
| Week 8 (10/9, 10/11, 10/13)   | [Arithmetic: Part 2][week 08 url]         | [Read/HW 08][read 08 url] | 10/15, 11:59PM |
| Week 9 (10/16, 10/18, 10/20)  | [The Processor: Part 1][week 09 url]      | [Read/HW 09][read 09 url] | 10/22, 11:59PM |
| Week 10 (10/23, 10/25, 10/27) | [The Processor: Part 2][week 10 url]      | [Read/HW 10][read 10 url] | 10/29, 11:59PM |
| Week 11 (10/30, 11/1, 11/3)   | [Memory Hierarchy: Part 1][week 11 url]   | [Read/HW 11][read 11 url] | 11/5, 11:59PM  |
| Week 12 (11/6, 11/8)          | [Memory Hierarchy: Part 2][week 12 url]   | [Read/HW 12][read 12 url] | 11/12, 11:59PM |
| Week 13 (11/13, 11/15, 11/17) | [Parallel Processes: Part 1][week 13 url] | [Read/HW 13][read 13 url] | 11/19, 11:59PM |
| Week 14 (11/20, 11/22)        | [Parallel Processes: Part 2][week 14 url] | [Read/HW 14][read 14 url] | 11/26, 11:59PM |
| Week 15 (11/27, 11/29, 12/1)  | --                                        | --                        | --             |
| Week 16 (12/4, 12/6)          | Review                                    | --                        | --             |
| Study Days (12/8)             | --                                        | --                        | --             |


## Homework/Quizzes/Exam
| NAME                                                                                               | DATE ASSIGNED | DEADLINE        |
|----------------------------------------------------------------------------------------------------|---------------|-----------------|
| [Quiz01-1][Quiz01-1 url]                                                                           | 8/21          | 8/23, 9:30 AM   |
| [Quiz01-2][Quiz01-2 url]                                                                           | 8/23          | 8/25, 9:30 AM   |
| [Quiz01-3][Quiz01-3 url]                                                                           | 8/25          | 8/28, 9:30 AM   |
| [Quiz01-4][Quiz01-4 url]                                                                           | 8/28          | 8/30, 9:30 AM   |
| [Quiz02-1][Quiz02-1 url]                                                                           | 8/30          | 9/1, 9:30 AM    |
| [Quiz02-2a][Quiz02-2a url]                                                                         | 9/1           | 9/8, 9:30 AM    |
| [Quiz02-2b][Quiz02-2b url]                                                                         | 9/1           | 9/8, 9:30 AM    |
| [Quiz02-3a][Quiz02-3a url]                                                                         | 9/3           | 9/10, 9:30 AM   |
| [Quiz02-3b][Quiz02-3b url]                                                                         | 9/3           | 9/10, 9:30 AM   |
| [Quiz02-4a][Quiz02-4a url]                                                                         | 9/6           | 9/13, 9:30 AM   |
| [Quiz02-4b][Quiz02-4b url]                                                                         | 9/6           | 9/13, 9:30 AM   |
| [Quiz03-1a][Quiz03-1a url]                                                                         | 9/8           | 9/15, 9:30 AM   |
| [Quiz03-1b][Quiz03-1b url]                                                                         | 9/8           | 9/15, 9:30 AM   |
| [Quiz03-2][Quiz03-2 url]                                                                           | 9/11          | 9/18, 9:30 AM   |
| [Quiz04-1a][Quiz04-1a url]                                                                         | 9/13          | 9/20, 9:30 AM   |
| [Quiz04-1b][Quiz04-1b url]                                                                         | 9/13          | 9/20, 9:30 AM   |
| [Quiz04-3][Quiz04-3 url]                                                                           | 9/15          | 9/22, 9:30 AM   |
| [Quiz04-4a][Quiz04-4a url]                                                                         | 9/18          | 9/25, 9:30 AM   |
| [Quiz04-4b][Quiz04-4b url]                                                                         | 9/18          | 9/25, 9:30 AM   |
| [Quiz04-5][Quiz04-5 url]                                                                           | 9/20          | 9/27, 9:30 AM   |
| [Quiz04-6][Quiz04-6 url]                                                                           | 9/22          | 9/29, 9:30 AM   |
| [Quiz04-7][Quiz04-7 url]                                                                           | 9/25          | 10/2, 9:30 AM   |
| [Quiz05-1][Quiz05-1 url]                                                                           | 9/29          | 10/6, 9:30 AM   |
| [Quiz05-3][Quiz05-3 url]                                                                           | 10/6          | 10/13, 9:30 AM  |
| [Quiz05-4][Quiz05-4 url]                                                                           | 10/9          | 10/16, 9:30 AM  |
| [HW 1: Single Cycle Processor in SystemVerilog][HW 1: Single Cycle Processor in SystemVerilog url] | 10/9          | 11/13, 11:55 PM |
| [Exam 1: Part 1][Exam 1: Part 1 url]                                                               | 10/16         | 10/23, 11:55 PM |
| [Exam 1: Part 2][Exam 1: Part 2 url]                                                               | 10/16         | 10/23, 11:55 PM |
| [Quiz06-1][Quiz06-1 url]                                                                           | 10/25         | 11/1, 9:30 AM   |
| [Quiz06-2][Quiz06-2 url]                                                                           | 11/1          | 11/8, 9:30 AM   |
| [Quiz06-3][Quiz06-3 url]                                                                           | 11/8          | 11/15, 9:30 AM  |
| [Exam II: Part A][Exam II: Part A url]                                                             | 11/20         | 11/27, 11:55 PM |
| [Exam II: Part B][Exam II: Part B url]                                                             | 11/20         | 11/27, 11:55 PM |
| [Quiz07-1][Quiz07-1 url]                                                                           | 11/22         | 11/29, 9:30 AM  |
| [Quiz07-2a][Quiz07-2a url]                                                                         | 11/27         | 12/4, 9:30 AM   |
| [Quiz07-2b][Quiz07-2b url]                                                                         | 11/27         | 12/4, 9:30 AM   |
| [Quiz07-3][Quiz07-3 url]                                                                           | 11/29         | 12/6, 9:30 AM   |
| [FINAL EXAM: Part A][FINAL EXAM: Part A url]                                                       | 12/8          | 12/15, 11:55 PM |
| [FINAL EXAM: Part B][FINAL EXAM: Part B url]                                                       | 12/8          | 12/15, 11:55 PM |


## Laboratory
| TIME            | Materials                                    | Virtual               | DEADLINE   |
|-----------------|----------------------------------------------|-----------------------|------------|
| Week 1 (8/22)   | [Unix Lab][lab 01 url]                       | [Vlab 01][vlab01 url] | 8/30, BOS  |
| Week 2 (8/29)   | [C Language][lab 02 url]                     | [Vlab 02][vlab02 url] | 9/12, BOS  |
| Week 3 (9/5)    | [C Language][lab 02 url]                     | [Vlab 02][vlab02 url] | 9/12, BOS  |
| Week 4 (9/12)   | [System Verilog 1][lab 03 url]               | [Vlab 03][vlab03 url] | 9/26, BOS  |
| Week 5 (9/19)   | [System Verilog 1][lab 03 url]               | [Vlab 03][vlab03 url] | 9/26, BOS  |
| Week 6 (9/26)   | [QtSPIM & MIPS][lab 04 url]                  | [Vlab 04][vlab04 url] | 10/10, BOS |
| Week 7 (10/3)   | [QtSPIM & MIPS][lab 04 url]                  | [Vlab 04][vlab04 url] | 2/28, BOS  |
| Week 8 (10/10)  | [FPGAs][lab 05 url]                          | [Vlab 05][vlab05 url] | 10/24, BOS |
| Week 9 (10/17)  | [FPGAs][lab 05 url]                          | [Vlab 05][vlab05 url] | 10/24, BOS |
| Week 10 (10/24) | [CPU Research][lab 06 url]                   | [Vlab 06][vlab06 url] | 11/7, BOS  |
| Week 11 (10/31) | [CPU Research][lab 06 url]                   | [Vlab 06][vlab06 url] | 11/7, BOS  |
| Week 12 (11/7)  | [Pipeline Processor][lab 07 url]             | [Vlab 07][vlab07 url] | 11/21, BOS |
| Week 13 (11/14) | [Pipeline Processor][lab 07 url]             | [Vlab 07][vlab07 url] | 11/21, BOS |
| Week 14 (11/21) | [SystemVerilog Hardware Threads][lab 08 url] | [Vlab 08][vlab08 url] | 12/5, BOS  |
| Week 15 (11/28) | [SystemVerilog Hardware Threads][lab 08 url] | [Vlab 08][vlab08 url] | 12/5, BOS  |
| Week 16 (12/5)  | --                                           | --                    | --         |
| Week 17 (12/12) | --                                           | --                    | --         |


***
<!-- # Resources
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
- [Verilog Full Reference](https://sutherland-hdl.com/pdfs/verilog_2001_ref_guide.pdf) -->



<!-- NOT DONE -->
[week urls]: # (week urls)
[week 1 url]:
[week 2 url]:
[week 3 url]:
[week 4 url]:
[week 5 url]:
[week 6 url]:
[week 7 url]:
[week 8 url]:
[week 9 url]:
[week 10 url]:
[week 11 url]:
[week 12 url]:
[week 13 url]:
[week 14 url]:

<!-- [recording urls]: # (recording urls) -->


<!-- DONE -->
[read urls]: # (reading urls)
[read 01 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/1/section/1
[read 02 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/2/section/1
[read 03 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/3/section/1
[read 04 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/4/section/1
[read 05 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/5/section/1
[read 06 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/6/section/1
[read 07 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/7/section/1
[read 08 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/8/section/1
[read 09 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/9/section/1
[read 10 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/10/section/1
[read 11 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/11/section/1
[read 12 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/12/section/1
[read 13 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/13/section/1
[read 14 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/14/section/1
[read 15 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/15/section/1
[read 16 url]: https://learn.zybooks.com/zybook/LandikaCOD(MIPS)Jun2023/chapter/16/section/1


[quiz urls]: # (quiz urls)
[quiz01-1 url]: 
[Quiz01-1 url]:
[Quiz01-2 url]:
[Quiz01-3 url]:
[Quiz01-4 url]:
[Quiz02-1 url]:
[Quiz02-2a url]:
[Quiz02-2b url]:
[Quiz02-3a url]:
[Quiz02-3b url]:
[Quiz02-4a url]:
[Quiz02-4b url]:
[Quiz03-1a url]:
[Quiz03-1b url]:
[Quiz03-2 url]:
[Quiz04-1a url]:
[Quiz04-1b url]:
[Quiz04-3 url]:
[Quiz04-4a url]:
[Quiz04-4b url]:
[Quiz04-5 url]:
[Quiz04-6 url]:
[Quiz04-7 url]:
[Quiz05-1 url]:
[Quiz05-3 url]:
[Quiz05-4 url]:
[HW 1: Single Cycle Processor in SystemVerilog url]:
[Exam 1: Part 1 url]:
[Exam 1: Part 2 url]:
[Quiz06-1 url]:
[Quiz06-2 url]:
[Quiz06-3 url]:
[Exam II: Part A url]:
[Exam II: Part B url]:
[Quiz07-1 url]:
[Quiz07-2a url]:
[Quiz07-2b url]:
[Quiz07-3 url]:
[FINAL EXAM: Part A url]:
[FINAL EXAM: Part B url]:


<!-- DONE -->
[labs urls]: # (labs urls) 
[lab 01 url]: https://drive.google.com/drive/folders/1RUZBkbuR70UuLQE-Srcy1ElGdnw7FVTI?usp=sharing
[lab 02 url]: https://drive.google.com/drive/folders/1XPCOLs0vI_3D02Sqs5alqeottEj5L8wQ?usp=sharing
[lab 03 url]: https://drive.google.com/drive/folders/1H_XGDP713rzK_TVmc_j5kR6RFFuH7f9c?usp=sharing
[lab 04 url]: https://drive.google.com/drive/folders/1Ra5vBMJaOnBi-8GG6U2FlFW-HKJZMBvT?usp=sharing
[lab 05 url]: https://drive.google.com/drive/folders/10nWKGHZ1zGnNgCI1KMMXUW6AiveuHwSC?usp=sharing
[lab 06 url]: https://drive.google.com/drive/folders/1ORI30YJMb6ZWit1huqsBpmc38s7L-4ze?usp=sharing
[lab 07 url]: https://drive.google.com/drive/folders/1B5wBi8XLgxAJXB2zaNuxtLCQl-AchXvq?usp=sharing
[lab 08 url]: https://drive.google.com/drive/folders/1B5wBi8XLgxAJXB2zaNuxtLCQl-AchXvq?usp=sharing


[vlabs urls]: # (vlabs urls)
[vlab01 url]: 
[vlab02 url]: 
[vlab03 url]: 
[vlab04 url]: 
[vlab05 url]: 
[vlab06 url]: 
[vlab07 url]: 
[vlab08 url]: 




<!-- NOT DONE -->
<!-- [resource urls]: # (resource urls)
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
[atom markdown enhanced url]: https://atom.io/packages/markdown-preview-enhanced -->
