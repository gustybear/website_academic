+++
title = "EE660: Computer Architecture"
subtitle = "Fall, 2018, with labs"
date = 2018-08-19T00:00:00-10:00
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["digital design", "fpga", "featured"]
+++

***
Fundamental understanding of computer architecture is key to hardware and processor design, compilers, operating systems, and high performance programming. This course explores computer architectures and design techniques of modern microprocessors at various scales. The focus will be given to architectures that can exploit different forms of parallelism, whether they be implicit or explicit, to improve performance. A selection of topics covered by the course include multi-issue superscalar processors, out-of-order processors, Very Long Instruction Word (VLIW) processors, advanced caching, multiprocessor systems, and parallel programming.

The function and operation of programmable logic devices, such as field programmable gate arrays (FPGAs), will be described and discussed in terms of how an HDL logic design is mapped and implemented. Experiments involving the design of various processors will provide students a hand-on introduction to computer engineering concepts and the skills needed to gain more advanced skills. In the laboratory, students will construct, troubleshoot, and test the computer processors that they have developed using a hardware description language. These custom designs will be implemented using FPGAs and validated using test equipment.

***
## Textbook
- *Required*: Computer Architecture: A Quantitative Approach (6th Edition).
- *Optional*: Modern Processor Design: Fundamentals of Supperscalar Processors.
- *Optional*: FPGA Prototyping By Verilog Examples: Xilinx Spartan-3 Version.

***
## Logistics
- *Lecturer*: [Yao Zheng](mailto:yao.zheng@hawaii.edu)
- *Lecture Time*: Mondays and Wednesdays, 9:00am-10:15am, Holmes Hall 241.
- *Lab Time*: TBD
- *Office hours*: Mondays and Wednesdays 11:00am-12:00pm or email for appointment, Holmes Hall 437

***
## Grading Policy
| Homework | Labs | Discussion | Midterms     | Final |
|----------|------|------------|--------------|-------|
| 25%      | 25%  | 10%        | 20%          | 20%   |


| A+   | A   | A-  | B+  | B   | B-  | C+  | C   | C-  | D+  | D   | D-  | F |
|------|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|---|
| 100% | 95% | 90% | 87% | 83% | 80% | 77% | 73% | 70% | 67% | 63% | 60% | 0 |


- *Homework*: You are encouraged to discuss homework assignments with your classmates and the course staff. Discussions may include general approaches to a problem, suggested resource material and whether your final answer is correct or not. However, each student must hand in their own implementation of the homework. **Copying of homework or code will result in a grade of zero for all parties involved**.

- *Labs*: In the lab you may work in teams of two. You may discuss the general approach to the lab assignment with other teams. However, each team must implement their own solution to the lab. Both team members must attend lab and sign-off. Each team must complete any pre-lab assignments individually and must submit them with their teams lab report. Duplication of code and/or data among teams will result in a grade of zero for all students involved.

- *Exams*: All exams are strictly individual efforts. Copying or otherwise cheating on an exam will result in a failing grade for the course.

***
## Schedule

| TIME    | TOPIC                                                | LECTURE                                       | LABORATORY           | READING                              | ASSG                   |
|---------|------------------------------------------------------|-----------------------------------------------|----------------------|--------------------------------------|------------------------|
| Week 1  | Introduction to Computer Architecture                | [lec 01][lec 01 url]                          | --                   | PH11: Chapter 1, C1-C16.             | --                     |
| Week 2  | Review: Pipeline                                     | [lec 02][lec 02 url]                          | --                   | PH11: C26, C30-C58, C61-C81.         | [assg 01][assg 01 url] |
| Week 3  | Review: Cache                                        | [lec 03][lec 03 url]                          | [lab 01][lab 01 url] | PH11: B1-B40, SL13:177-209.          | --                     |
| Week 4  | Out-of-Order Processors                              | [lec 04a][lec 04a url] [lec 04b][lec 04b url] | --                   | PH11:C43-C61, SL13:217-236.          | --                     |
| Week 5  | Branch, Register Renaming, and Memory Disambiguation | [lec 05][lec 05 url]                          | --                   | SL13:237-273.                        | --                     |
| Week 6  | VLIW Introduction                                    | [lec 06][lec 06 url]                          | --                   | PH11: 192-196, Appendix H            | --                     |
| Week 7  | Branch Prediction, Advanced Cache Optimizations      | [lec 07a][lec 07a url] [lec 07b][lec 07b url] | --                   | PH11: C26-C30, SL13:219-237, 453-508 | [assg 02][assg 02 url] |
| Week 8  | Memory Protection                                    | [lec 08][lec 08 url]                          | [lab 02][lab 02 url] | PH11:B41,B67,105-144                 | --                     |
| Week 9  | Vector Processors and GPUs                           | [lec 09a][lec 09a url] [lec 09b][lec 09b url] | --                   | PH11:344-412                         | --                     |
| Week 10 | Course Project (Preliminary Presentation)            | [prj repo][prj 01 url]                        | --                   | --                                   | --                     |
| Week 11 | Multithreading                                       | [lec 10][lec 10 url]                          | --                   | PH11:221-259                         | --                     |
| Week 12 | Parallel Programming and Small Multiprocessors       | [lec 11][lec 11 url]                          | --                   | PH11:386-400, 343-378                | --                     |
| Week 13 | Interconnection Network                              | [lec 12][lec 12 url]                          | --                   | PH11:Appendix F                      | [assg 03][assg 03 url] |
| Week 14 | Large Multiprocessors (Directory Protocols)          | [lec 13][lec 13 url]                          | [lab 03][lab 03 url] | PH11:378-386, 400-429                | --                     |
| Week 15 | USRP and Wireless Security, Part 1                   | [lec 14][lec 14 url]                          | --                   | --                                   | --                     |
| Week 16 | USRP and Wireless Security, Part 2                   | [lec 15][lec 15 url]                          | --                   | --                                   | --                     |
| Week 17 | Final Project Presentations                          | --                                            | --                   | --                                   | --                     |

## Resources
- [Xilinx Vivado HL Webpack Installation Guide][xilinx vivado tutorial]
- [Hardware Menu][hardware menu url]
- [Software Menu][software menu url]
- [Troubleshoot][troubleshoot url]

[lec urls]: # (lec urls)
[lec 01 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_01_slides.pdf
[lec 02 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_02_slides.pdf
[lec 03 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_03_slides.pdf
[lec 04a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_04_slides_a.pdf
[lec 04b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_04_slides_b.pdf
[lec 05 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_05_slides.pdf
[lec 06 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_06_slides.pdf)
[lec 07a url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_07_slides_a.pdf)
[lec 07b url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_07_slides_b.pdf)
[lec 08 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_08_slides.pdf)
[lec 09a url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_09_slides_a.pdf)
[lec 09b url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_09_slides_b.pdf)
[lec 10 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_11_slides.pdf)
[lec 11 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_12_slides.pdf)
[lec 12 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_13_slides.pdf)
[lec 13 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_14_slides.pdf)
[lec 14 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_15_slides_a.pdf)
[lec 15 url]: # (https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2018_fall/docs/slides/ee660_2018_fall_materials_week_15_slides_b.pdf)

[lab urls]: # (lab urls)
[lab 01 url]: ./laboratories/01/
[lab 02 url]: ./laboratories/02/
[lab 03 url]: # (tbd)

[assg urls]: # (assg urls)
[assg 01 url]: ./assignmentgs/01/
[assg 02 url]: # (tbd)
[assg 03 url]: # (tbd)

[prj urls]: # (prj urls)
[prj 01 url]: # (tbd)

[resource urls]: # (resource urls)
[xilinx vivado tutorial]: ./tutorials/01/
[hardware menu url]: # (tbd)
[software menu url]: # (tbd)
[troubleshoot url]: # (tbd)
