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
- *Teaching Assistant(s)*: [Marionne Millan](mailto:marionne@hawaii.edu)
- *Grader(s)*: N/A
- *Lecture Time*: Mondays, Wednesdays, and Fridays 9:30am-10:20am, Kuykendall Hall 305.
- *Lab Time*: Tuesdays 9:00am-11:45am or 1:30pm-4:15pm, Holmes Hall 451.
- *Office hours*: see [here](../../#contact).

***
# Textbook
- *Required*: [EE 260: Introduction to Digital Design](https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021), by Zybooks
  - Buy at [ZyBooks](https://learn.zybooks.com/zybook/HAWAIIEE260ZhengSpring2021)
  - [How to use Zybooks](https://learn.zybooks.com/zybook/HowToUseZyBooks2)
- *Optional*: [Digital Design Principles and Practice with Verilog (5th Edition)](https://www.pearson.com/us/higher-education/program/Wakerly-Digital-Design-Principles-and-Practices-5th-Edition/PGM337271.html), by John F. Wakerly.
  - Buy at [Amazon](https://www.amazon.com/Digital-Design-Principles-Practices-5th/dp/013446009X/ref=sr_1_1?ie=UTF8&qid=1546977313&sr=8-1&keywords=Digital+Design+Principles+and+Practice).
  - By at UHM Bookstore.
  - Library Reserve (Sinclair Library Wong Audiovisual Center, Call#: TK7874.65 .W34 2018).
- *Optional*: [Digital Design with RTL Design, VHDL, and Verilog (2nd Edition)](http://bcs.wiley.com/he-bcs/Books?action=index&itemId=0470531088&bcsId=5568), by Frank Vahid.
  - Buy at [Amazon](https://www.amazon.com/Digital-Design-RTL-VHDL-Verilog/dp/0470531088/ref=sr_1_1?keywords=Digital+Design+with+RTL+Design%2C+VHDL%2C+and+Verilog+%282nd+Edition%29&qid=1578885767&sr=8-1).
  - Library Reserve (Hamilton Library Circulation, Call # -  TK7888.3 .V274 2011).
- *Optional*: [FPGA Prototyping By Verilog Examples: Xilinx Spartan-3 Version (1st Edition)](https://academic.csuohio.edu/chu_p/rtl/fpga_vlog.html), by Pong P. Chu.
- *Optional*: [FPGA Prototyping by SystemVerilog Examples: Xilinx MicroBlaze MCS SoC Edition (2nd Edition)](https://academic.csuohio.edu/chu_p/rtl/fpga_mcs_sv.html), by Pong P. Chu.

***
# Xilinx Vivado and Basys3 
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
### Rubric
| Problem | Unacceptable(0) | Marginal(1) | Acceptable(2) | Very Good(3) | Excellent(4) |
| --- | --- | --- | --- | --- | --- |
| Rubric A:Skills Problems |   - Missing or minor attempt at the problem.<br> - No description of problem or method of solution.<br> - Most results are incorrect.<br> - Missing major concepts for the problem.<br>   |   - Problem statement missing or unclear.<br> - Many incorrect results due to missing concepts.<br> - Little work shown to illustrate understanding.<br>   |   - Problem statement identified.<br> - Some incorrect results due to minor errors.<br> - Steps to solution shown in some cases.<br>   |   - Problem statement stated in the solution.<br> - Results are correct in almost all cases.<br> - Sufficient work shown to understand how results obtained.<br> - Clearly understands most concepts.<br>   |   - Problem statement clearly stated in the solution.<br> - Results are correct in all cases.<br> - Derivation of results neat, clear and easy to follow.<br> - Clearly understands all concepts.<br>   |
| Rubric B:Design Problems |   - Missing or minor attempt at the problem.<br> - Major issues or concepts missing in solution.<br> - No or few figures or non-understandable or missing labels on figures.<br> - No description of reasoning in the design or design choices.<br> - Little or no evidence of a design process.<br>   |   - A slight attempt at the problem.<br> - Limited evidence or weak description of organized design process.<br> - Figures hard to understand, mostly unlabeled, not well described.<br>   |   - A reasonable approach to the problem.<br> - Some evidence and description of process used in the design.<br> - Good figures, somewhat labeled and described.<br>   |   - A good approach to the problem.<br> - Documentation mostly complete and in logical order.<br> - Good evidence and description of process used in the design.<br> - Clear figures, mostly labeled and described.<br>   |   - Well documented, correct, complete and understandable design.<br> - Systematic design process clearly evident.<br> - Good figures used where appropriate.<br> - Figures and signals labeled and described.<br> - Some evidence of alternatives considered.<br> - Possible creative or unique approach to the problem.<br>   |
| Rubric C:Schematic Drawing Problems |   - Design missing, incomplete or doesn't meet spec.<br> - Layout sloppy, does not follow conventions or missing connections.<br> - Design doesn't work.<br>   |   - Design mostly complete, but not ready for simulation.<br> - Some simulation problems, but works in some cases.<br> - Layout sloppy, not follow conventions or missing connections.<br>   |   - Design mostly complete and ready for simulation.<br> - Only minor problems in simulation, works in most cases.<br> - Layout is neat and clean; mostly follows conventions.<br>   |   - Design complete, and ready for simulation.<br> - Simulation works in almost all cases.<br> - Layout is neat and clean; follows conventions.<br>   |   - Design is complete and ready for simulation.<br> - Simulation works and meets spec.<br> - Layout is very clear, well labeled and easy to follow.<br>   |
| Rubric D:Analysis Problems |   - Analysis missing or incomplete.<br> - Missed most major features of the system.<br> - Writeup is unorganized and sloppy.<br>   |   - Some attempt at understanding the system.<br> - Missed some major features of the system or not sufficiently specific.<br> - Unimportant features misclassified as important.<br> - Writeup is hard to follow and understand.<br>   |   - Reasonable understanding of the system being analyzed; some misconceptions.<br> - Describes most of the important features of the system in some detail.<br> - Pretty good organization and flow of ideas.<br>   |   - Good understanding of the system being analyzed.<br> - Describes all of the important features of the system in good detail.<br> - Very good organization and flow of ideas.<br>   |   - Evidence that the system being analyzed is well understood.<br> - Analysis clear, organized and complete.<br> - Important points are identified and well explained.<br>   |
| Rubric E:Assignment Organization & Presentation |  - Much of assignment missing or incomplete.<br> - Work submitted is sloppy or unorganized.<br> - No attempt to follow the spec or documentation standards.<br> - Little effort evident in the assignment.<br>   |   - Assignment mostly complete, but missing some elements.<br> - Organization hard to follow or does not follow spec.<br> - Insufficient effort to make solutions clear.<br>   |   - Assignment is mostly complete, in one document with appropriate support files.<br> - Document mostly well organized, but not quite to spec.<br> - Solutions are in order, identified and reasonable to follow.<br> - Reasonably well written, but some unstated assumptions.<br>   |   - Assignment is complete, in one correctly named document with appropriate support files.<br> - Document well organized, follows spec.<br> - Solutions are easy to find and identify, and clear to follow.<br> - Mostly well written and clear.<br>   |   - Complete assignment submitted as one document with appropriate support files.<br> - Document well organized as specified, including file names.<br> - Well written and easy to understand.<br>   |
| Rubric F:Teamwork Process |   - No description of teamwork process.<br> - Little collaboration or coordination on the team.<br> - One or two members doing all or most of the work.<br>   |   - Team having difficulties communicating and coordinating the assignment.<br> - Most members of the team do their own thing and send it in.<br>   |   - Reasonable distribution of workload on the team.<br> - Team works together and tries to check each other's work and understanding.<br> - Some small problems in the team, but working on them.<br>   |   - Good distribution of workload on the team and well documented.<br> - Most team members contributed to the solutions.<br> - Most team members exercised a variety of skills.<br> - Team works well together to check each other's work and understanding.<br> - No issues with team communication.<br>   |   - All team members clearly contributed to the solutions.<br> - All team members exercised a variety of skills.<br> - All evals turned in on time.<br> - Team is communicating well and operating smoothly.<br> - A well oiled machine.<br>   |
| Rubric G:Vivado and Basys3 Lab Problems |   - Design missing, incomplete or doesn't meet spec.<br> - VHDL doesn't compile or synthesize.<br> - Design doesn't work.<br>   |   - Design mostly complete, but not ready for simulation.<br> - Some simulation problems, but works in some cases.<br>   |   - Design mostly complete, and ready for simulation.<br> - Only minor problems in simulation.<br> - Inputs and outputs follow spec, but hard to use.<br>   |   - Design is complete and ready for simulation.<br> - Simulation works after a little tweaking and meets mostly spec.<br> - Inputs and Outputs labeled and easy to use.<br>   |   - Design is complete and ready for simulation.<br> - Simulation works very well and completely meets spec.<br> - Inputs and Outputs well labeled and easy to use.<br> - Demo well presented.<br>   |

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
| TIME                                            | LECTURE                                                             | LABORATORY                                 | READING                        | ASSIGMENT                                     | DUE (before first lecture) |
| ---                                             | ---                                                                 | ---                                        | ---                            | ---                                           | ---                        |
| [Week 1 (1/11. 1/13, 1/15)][week 01 url]          | Course Logistic and Introduction                                    |                                            | zyBooks Week 01                |                                               | --                         |
| [Week 2 (1/20. 1/22)][week 02 url]              | Number Systems                                                      | Vivado Tutorial                            | zyBooks Week 02                | Numbering Systems                             | --                         |
| [Week 3 (1/25. 1/27, 1/29)][week 03 url]          | Combinational Logic: Switches, Transistors, Logic Gates             | Modeling Concepts                          | zyBooks Week 03                | Switches, Transistors, Logic Gates            | Week 1                     |
| [Week 4 (2/1, 2/3, 2/5)][week 04 url]          | Combinational Logic: Boolean Algebra                                | Numbering Systems                          | zyBooks Week 04                | Boolean Algebra                               | Week 2                     |
| [Week 5 (2/8, 2/10, 2/12)][week 05 url]          | Combinational Logic: Design Process, More Gates                     | Multi-Output Circuits                      | zyBooks Week 05                | Design Process, More Gates                    | Week 3                     |
| Week 6 (Feb 17)                                 | Review: Combinational Logic                                         |                                            |                                |                                               | Week 4                     |
| [Week 6 (Feb 19)][week 06 url]                  | Midterm I: Computer allowed.                                        | At home.                                   | 9:30AM - 10:45AM               |                                               |                            |
| [Week 7 (2/22, 2/24, 2/26)][week 07 url]          | Review: Midterm I, Sequential Logic: Clock, Latches, and Flip-Flops | Tasks Functions, and Testbench             | [zyBooks Week 07][read 07 url] | Latches and Flip-Flops                        | Week 5                     |
| [Week 8 (3/1, 3/3, 3/5)][week 08 url]          | Sequential Logic: Finite State Machines                             | Modeling Latches and Flip-Flops            | [zyBooks Week 08][read 08 url] | Finite State Machines                         | --                         |
| [Week 9 (3/8, 3/10, 3/12)][week 09 url]          | Sequential Logic: Registers, Counters, Shifters, and Arithmetic     | Finite State Machines                      | [zyBooks Week 09][read 09 url] | Registers, Counters, Shifters, and Arithmetic | Week 7                     |
| Spring Recess (Mar 15  - Mar 19)                |                                                                     |                                            |                                |                                               |
| Week 10 (Mar 22)                                | Review: Sequential Logic                                            |                                            |                                |                                               | Week 8                     |
| [Week 10 (Mar 24)][week 10 url]                 | Midterm Exam II:          Computer allowed.                         | At home.                                   | 9:30AM - 10:45AM               |                                               |
| [Week 11 (3/29, 3/31)][week 11 url] | Register-Transfer Level Design                                      | Modeling Registers and Counters            | [zyBooks Week 11][read 11 url] | Register-Transfer Level Process               | Week 9                     |
| [Week 12 (4/5, 4/7, 4/9)][week 12 url]             | Register Memory Components and FIFO                                 | Architectural Wizard and IP Catalog        | [zyBooks Week 12][read 12 url] | Register Files, Cache, and Memory Components  | --                         |
| [Week 13 (4/12, 4/14, 4/16)][week 13 url]         | Optimizations and Tradeoffs                                         | Behavioral Modeling and Timing Constraints | [zyBooks Week 13][read 13 url] | Optimizations and Tradeoffs                   | Week 11                    |
| [Week 14 (4/19, 4/21, 4/23))][week 14 url]         | Physical Implementation on ICs                                      | Sequential System Design using ASM Charts  | [zyBooks Week 14][read 14 url] | Physical Implementation on ICs                | Week 12                    |
| [Week 15 (4/26, 4/28, 4/30)][week 15 url]     | Programmable Processors                                             | Catch-up Lab                               | [zyBooks Week 15][read 15 url] | Programmable Processors                       | Week 13                    |
| [Week 16 (May 03, 05)][week 16 url]             | Class Review                                                        |                                            |                                |                                               | Week 14                    |
| Study Days (May 07, 08)                         |                                                                     |                                            |                                |                                               |
| [Week 17 (May 10)][week 17 url]                 | Final:       Computer allowed                                       | Kuykendall Hall 305                        | 9:45AM - 11:45AM               |                                               | Week 15                    |

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
