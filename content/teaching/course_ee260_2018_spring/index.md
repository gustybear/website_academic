+++
draft = true
title = "EE260: Introduction to Digital Design (Spring, 2018)"
date =  2017-12-31T00:00:00-10:00
+++

***
Digital circuits are the foundations to build calculators, computers and cell phones, etc. This course explores these foundations by using modern digital design techniques to design, implement and test digital circuits ranging from basic logic gates to state machines that perform useful functions like calculations, counting, timing, and a host of other applications. Students will learn modern design techniques, using a hardware description language (HDL) such as Verilog to design, simulate and implement logic systems consisting of basic gates, adders, multiplexers, latches, counters, and basic processors.

The function and operation of programmable logic devices, such as field programmable gate arrays (FPGAs), will be described and discussed in terms of how an HDL logic design is mapped and implemented. Experiments involving the design of combinational and sequential circuits will provide students a hand-on introduction to basic digital electrical engineering concepts and the skills needed to gain more advanced skills. In the laboratory, students will construct, troubleshoot, and test the digital circuits that they have developed using a hardware description language. These custom logic designs will be implemented using FPGAs and validated using test equipment.

***
## Textbook
- *Required*: Digital Design Principles and Practice with Verilog (5th Edition).
- *Optional*: FPGA Prototyping By Verilog Examples: Xilinx Spartan-3 Version.

***
## Logistics
- *Lecturer*: [Yao Zheng](mailto:yao.zheng@hawaii.edu)
- *Teaching Assistant*: [Joshua Chen](mailto:jschen2@hawaii.edu)
- *Grader*: [Nicolas Yama](mailto:nyama8@hawaii.edu)
- *Lecture Time*: Mondays, Wednesdays, and Fridays 9:30am-10:20am, Marine Science Building 100.
- *Lab Time*: Tuesdays 9:00am-11:45am, Holmes Hall 451.
- *Office hours*: Mondays and Wednesdays 14:00pm-16:00pm or email for appointment, Holmes Hall
437.

***
## Grading Policy
| Homework | Labs | Discussion | Midterms (2) | Final |
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
TIME                            | TOPIC                                                                      | LECTURE                                                                         | LABORATORY                                               | READING                                             | ASSG
--------------------------------|----------------------------------------------------------------------------|---------------------------------------------------------------------------------|----------------------------------------------------------|-----------------------------------------------------|--------------------------------------------
Week 1 (Jan 8, 10)              | Introduction                                                               | [lec 01][lec 01 url]                                                            | [lab 1][lab 1 url] (due 23:59PM Jan 21)                  | Wakerly Ch. 1                                       |
Week 2 (Jan 17, 19)             | Number Systems                                                             | [lec 02][lec 02 url]                                                            | [lab 2][lab 2 url] (due 23:59PM Feb 4)                   | Wakerly Sec. 2.1 - Sec. 2.6                         | [assg 01][assg 01 url] (due 23:59PM Jan 28)
Week 3 (Jan 22, 24, 26)         | Boolean Algebra: Logic Representations and Analysis                        | [lec 03][lec 03 url]                                                            | [lab 2 sup][lab 2 sup url] (due 23:59PM Feb 4)           | Wakerly Sec. 3.1 - Sec. 3.3                         | [assg 02][assg 02 url] (due 23:59PM Feb 4)
Week 4 (Jan 29, 31, Feb 2)      | Boolean Algebra: Logic Synthesis and Timing Hazards                        | [lec 04][lec 04 url]                                                            | [lab 3][lab 3 url] (due 23:59PM Feb 18)                  | Wakerly Sec. 4.1, 4.2, 3.3 [ezpixel][ezpixel url]   | [assg 03][assg 03 url] (due 23:59PM Feb 11)
Week 5 (Feb 5, 7, 9)            | Verilog HDL: Basic                                                         | [lec 05][lec 05 url]                                                            |                                                          | Wakerly Sec. 15.5, 5.1 - 5.4                        | [quiz 1][quiz 1 url] (due 10:20AM Feb 9)
Midterm Exam I (Feb 12)         | Closed Book & Notes. One page of notes allowed. No calculators             | [midterm 1 sol][midterm 1 sol url]                                              |                                                          |                                                     |
Week 6 (Feb 14, 16)             | Combinational Circuits: MUXs, Encoders, Decoders, Priority Encoders        | [lec 06][lec 06 url]                                                            | [lab 4][lab 4 url] (due 23:59PM Mar 4)                   | Wakerly Sec. 6.3, 6.4, 7.2                          | [assg 04][assg 04 url] (due 23:59PM Feb 27)
Week 7 (Feb 21, 23)             | Combinational Circuits: Three-State Devices, Parity Functions, Comparators | [lec 07][lec 07 url]                                                            | [lab 4 sup][lab 4 sup url] (due 23:59PM Mar 4)           | Wakerly Sec. 7.1, 7.3, 7.4                          | [assg 05][assg 05 url] (due 23:59PM Mar 4)
Week 8 (Feb 26, 28, Mar 2)      | Combinational Circuits: Adders, Subtractors                                | [lec 08][lec 08 url] [assg 05 review][assg 05 review url]                       | [lab 5][lab 5 url] (due 23:59PM Mar 21)                  | Wakerly Sec. 8.1                                    | [assg 06][assg 06 url] (due 23:59PM Mar 11)
Week 9 (Mar 5, 7, 9)            | Combinational Circuits: Multipliers. Dividers, Shifters                    | [lec 09][lec 09 url]                                                            | [lab 5: displaycontroller][lab 5: displaycontroller url] | Wakerly Sec. 8.2, 8.3, 8.4                          | [assg 07][assg 07 url] (due 23:59PM Mar 21)
Week 10 (Mar 12, 14, 16)        | Combinational Circuits: Memory, Combinational Datapath                     | [lec 10a][lec 10a url] [lec 10b][lec 10b url]                                   |                                                          | Wakerly Sec. 15.1 - 15.2                            |
Midterm Exam II (Mar 19)        | Closed Book & Notes. Computer allowed. No Internet.                        | [midterm 2 practice][midterm 2 practice url] [midterm 2 sol][midterm 2 sol url] |                                                          |                                                     |
Week 11 (Mar 21, 23)            | Verilog HDL: Combinational Circuits, Test Bench, etc.                      | [lec 11a][lec 11a url] [lec 11b][lec 11b url]                                   | [lab 6][lab 6 url] (due 23:59PM Apr 15)                  | [semiconductor reuse standard][srs url]             | [quiz 2][quiz 2 url] (due 10:20AM Apr 4)
Spring Recess (Mar 26 - Mar 30) |                                                                            |                                                                                 |                                                          |                                                     |
Week 12 (Apr 2, 4, 6)           | Sequential Circuits: Overview, Latches, Flip-Flops                         | [lec 12][lec 12 url]                                                            |                                                          | Wakerly Sec. 10.1 - 10.3                            | [assg 08][assg 08 url] (due 23:59PM Apr 15)
Week 13 (Apr 9, 11, 13)         | Sequential Circuits: Counters and Shift Registers                          | [lec 13][lec 13 url]                                                            | [lab 7][lab 7 url] (due 23:59PM May 6)                   | Wakerly Sec. 11.1 - 11.2                            | [assg 09][assg 09 url] (due 23:59PM Apr 22)
Week 14 (Apr 16, 18, 20)        | Sequential Circuits: State Machines                                        | [lec 14][lec 14 url]                                                            | [lab 8][lab 8 url] (due 23:59PM May 6)                   | Wakerly Sec. 9.1 - 9.4                              | [assg 10][assg 10 url] (due 23:59PM May 6)
Week 15 (Apr 23, 25, 27)        | Sequential Circuits: Sequential Circuit Design                             | [lec 15][lec 15 url]                                                            |                                                          | Wakerly Sec. 13.2 - 13.4                            |
Week 16 (Apr 30, Mar 2)         | Verilog HDL: Memory Interfaces, Embedded Processors etc.                   | [lec 16a][lec 16a url] [lec 16b][lec 16b url]                                   |                                                          | [micron cellular ram][mcr url] [microblaze][mb url] | [quiz 3][quiz 3 url] (due 10:20AM May 2)
Study Days (May 3 - May 4)      |                                                                            | [practice exam][practice exam url]                                                  |                                                          |                                                     |
Final Exam (9:45AM May 7, MSB 100)              | Closed Book & Notes. Computer allowed. No Internet.                        |                                                                                 |                                                          |                                                     |

***
## Resources
- [Xilinx Vivado HL Webpack Installation Guide][xilinx vivado tutorial]
- [Hardware Menu][hardware menu url]
- [Software Menu][software menu url]
- [Troubleshoot][troubleshoot url]

[lec urls]: # (lec urls)
[lec 01 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_01_slides.pdf
[lec 02 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_02_slides.pdf
[lec 03 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_03_slides.pdf
[lec 04 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_04_slides.pdf
[lec 05 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_05_slides.pdf
[lec 06 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_06_slides.pdf
[lec 07 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_07_slides.pdf
[lec 08 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_08_slides.pdf
[lec 09 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_09_slides.pdf
[lec 10a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_10_slides_a.pdf
[lec 10b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_10_slides_b.pdf
[lec 11a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_11_slides_a.pdf
[lec 11b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_11_slides_b.pdf
[lec 12 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_12_slides.pdf
[lec 13 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_13_slides.pdf
[lec 14 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_14_slides.pdf
[lec 15 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_15_slides.pdf
[lec 16a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_16_slides_a.pdf
[lec 16b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_16_slides_b.pdf

[lab urls]: # (lab urls)
[lab 1 url]: https://classroom.github.com/a/3Vug4__H
[lab 2 url]: https://classroom.github.com/g/CZwoyb0X
[lab 2 sup url]: https://tinyurl.com/y7xfwwwy
[lab 3 url]: https://classroom.github.com/g/6pTJLIPt
[lab 4 url]: https://classroom.github.com/g/GLgyFyyy
[lab 4 sup url]: https://tinyurl.com/y9fzrpxp
[lab 5 url]: https://classroom.github.com/g/vi4bvpns
[lab 5: displaycontroller url]: https://raw.githubusercontent.com/ee260-2018-spring/ee260_2018_spring_materials_laboratory_05_repo/master/codes/displaycontrolller.v
[lab 6 url]: https://classroom.github.com/g/xSCfdPrN
[lab 7 url]: https://classroom.github.com/a/KGg4zeR-
[lab 8 url]: https://classroom.github.com/g/ToQm3aAb

[assg urls]: # (assg urls)
[assg 01 url]: https://classroom.github.com/a/yOMrBZHi
[assg 02 url]: https://classroom.github.com/a/Dt0YkFPp
[assg 03 url]: https://classroom.github.com/a/fAhaOeNV
[assg 04 url]: https://classroom.github.com/a/3w0n2ZcC
[assg 05 url]: https://classroom.github.com/a/dKAU7Q7F
[assg 05 review url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/ee260_2018_spring_materials_week_08_slides_assg.pdf
[assg 06 url]: https://classroom.github.com/a/XSZ_LTw6
[assg 07 url]: https://classroom.github.com/a/0E8Sof8b
[assg 08 url]: https://classroom.github.com/a/7OVQs8fO
[assg 09 url]: https://classroom.github.com/a/ypgRXzAp
[assg 10 url]: https://classroom.github.com/a/LJzIR4tr

[reading urls]: # (reading urls)
[ezpixel url]: https:s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/reading/Burke_2018_The%20ezPixel%20lights%20it%20up%20%5BResources%5D.pdf
[srs url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/FreescaleVerilog.pdf
[mcr url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/128mb_burst_cr1_5_p26z.pdf
[mb url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/slides/mb_ref_guide.pdf

[quiz urls]: # (quiz urls)
[quiz 1 url]: https://goo.gl/forms/XV7AGnrRRP9vxO242
[quiz 2 url]: https://goo.gl/forms/30AgmpUf8emeNjjF3
[quiz 3 url]: https://goo.gl/forms/SikmgVUQFCtdl23K3

[exam urls]: # (exam urls)
[midterm 1 sol url]: http://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee260_2018_spring/docs/exam-sol/ee260_2018_spring_materials_exam_01.pdf
[midterm 2 practice url]: https://classroom.github.com/a/Umy0O5Jq
[midterm 2 sol url]: https://github.com/ee260-2018-spring/ee260_2018_spring_materials_exam_02_repo
[practice exam url]: https://classroom.github.com/a/gH_ED48t

[resource urls]: # (resource urls)
[xilinx vivado tutorial]: ../tutorials/xilinx_vivado_installation_guide/
[hardware menu url]: # (tbd)
[software menu url]: # (tbd)
[troubleshoot url]: # (tbd)
