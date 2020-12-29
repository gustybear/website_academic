+++
draft = true
title = "EE660: Computer Architecture (Spring, 2017)"
date = 2017-06-01T00:00:00-10:00
+++
***
Fundamental understanding of computer architecture is key to hardware and processor design, compilers, operating systems,index and high performance programming. This course explores computer architectures and design techniques of modern microprocessors at various scales. Focus will be given to architectures that can exploit different forms of parallelism, whether they be implicit or explicit, to improve performance. A selection of topics covered by the course include multi-issue superscalar processors, out-of-order processors, Very Long Instruction Word (VLIW) processors, advanced caching, multiprocessor systems, and parallel programming.

The function and operation of programmable logic devices, such as field programmable gate arrays (FPGAs), will be described and discussed in terms of how an HDL logic design is mapped and implemented. Experiments involving the design of various processors will provide students a hand-on introduction to computer engineering concepts and the skills needed to gain more advanced skills. In the laboratory, students will construct, troubleshoot, and test the computer processors that they have developed using a hardware description language. These custom designs will be implemented using FPGAs and validated using test equipment.
***

**Lecturer**:
Yao Zheng (yao.zheng@hawaii.edu)

**Lecture**:
Mondays and Wednesdays 3:00pm-4:15am, Kuykendall 304.

**Office hours**:
Mondays to Fridays 14:00pm-16:00pm or email for appointment, Holmes Hall 437.

**Textbook**:
PH11 = Computer Architecture: A Quantitative Approach (5th Edition), 2011
SL13 = Modern Processor Design: Fundamentals of Superscalar Processors (1st Edition), 2005, reissued 2013.

**Syllabus**: here.

**Schedule**

TIME  | TOPIC | SLIDES | READING | ASSG
---   | ---   |:---    | ---     |  ---
Week 1 | Introduction to Computer Architecture | [slides 01](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_01_slides.pdf) | PH11: Chapter 1, C1-C16. | --
Week 2 | Review: Pipeline | [slides 02](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_02_slides.pdf) | PH11: C26, C30-C58, C61-C81. |  [assignment 01](https://classroom.github.com/a/ZbYaNI2q)
Week 3 | Review: Cache | [slides 03](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_03_slides.pdf) | PH11: B1-B40, SL13:177-209. | --
Week 4 | Out-of-Order Processors | [slides 04a](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_04_slides_a.pdf) [slides 04b](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_04_slides_b.pdf) | PH11:C43-C61, SL13:217-236. | --
Week 5 | Branch, Register Renaming, and Memory Disambiguation | [slides 05](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_05_slides.pdf) | SL13:237-273. | --
Week 6 | VLIW Introduction | [slides 06](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_06_slides.pdf) | PH11: 192-196, Appendix H | -- | --
Week 7 | Branch Prediction, Advanced Cache Optimizations | [slides 07a](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_07_slides_a.pdf) [slides 07b](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_07_slides_b.pdf) | PH11: C26-C30, SL13:219-237, 453-508| [assignment 02](https://classroom.github.com/a/qWw0pNfl)
Week 8  | Memory Protection | [slides 08](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_08_slides.pdf) | PH11:B41,B67,105-144 | -- | --
Week 9 | Vector Processors and GPUs | [slides 09a](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_09_slides_a.pdf) [slides 09b](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_09_slides_b.pdf) |PH11:344-412 | --
Week 10 | Course Project (Preliminary Presentation) | -- | -- |  [project repo](https://classroom.github.com/a/eRHkLZUE)
Midterm | [exam repo](https://classroom.github.com/a/uL9gG5cA) ||
Week 11 | Multithreading | [slides 10](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_11_slides.pdf) | PH11:221-259 | --
Week 12 | Parallel Programming and Small Multiprocessors | [slides 11](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_12_slides.pdf) | PH11:386-400, 343-378 | -- | --
Week 13 | Interconnection Network | [slides 12](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_13_slides.pdf) | PH11:Appendix F | --
Week 14 | Large Multiprocessors (Directory Protocols) | [slides 13](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_14_slides.pdf) | PH11:378-386, 400-429 |  --
Week 15 | Cloud Architecture and Hardware Security | [slides 14a](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_15_slides_a.pdf) [slides 14b](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_15_slides_b.pdf ) [slides 14c](https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2017_fall/docs/slides/ee660_2017_fall_materials_week_15_slides_c.pdf) | -- |[assignment 03](https://classroom.github.com/a/IeMzA8Fd) ||
Week 16 | Computer Architecture and Deep Learning | -- | -- | --
Week 17 | Final Project Presentations | -- | -- | -- | --

## Resources
- [Hardware Menu][hardware menu url]
- [Software Menu][software menu url]
- [Troubleshoot][troubleshoot url]

[resource urls]: # (resource urls)
[hardware menu url]: # (tbd)
[software menu url]: # (tbd)
[troubleshoot url]: # (tbd)
