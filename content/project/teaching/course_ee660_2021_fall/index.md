---
title: "EE660: Computer Architecture I"

subtitle: "Fall, 2021"

summary: "EE660 is the graduate-level course to study models of computation, high-performance processors, pipelined machines, RISC processors, VLIW, superscalar and fine-grain parallel machines."

date: 2021-08-02T10:07:39-10:00
lastmod: 2021-08-02T10:07:39-10:00
featured: false
draft: false

authors:
- Yao Zheng

tags:
- digital design
- fpga
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
- name: CRN
  url: ./project/teaching/course_ee660_2021_fall/#logistics
---

***
# Executive Summary
Fundamental understanding of computer architecture is key to hardware and processor design, compilers, operating systems, and high performance programming. This course explores computer architectures and design techniques of modern microprocessors at various scales. The focus will be given to architectures that can exploit different forms of parallelism, whether they be implicit or explicit, to improve performance. A selection of topics covered by the course include multi-issue superscalar processors, out-of-order processors, Very Long Instruction Word (VLIW) processors, advanced caching, multiprocessor systems, and parallel programming.
***

# Logistics {#logistics}
- **CRN**
| EE660 001 |
| ---   |
| 87637 |

- **Personnel**:
|                                                    |                                             |
| ----                                               | ---                                         |
| Lecturer: [Yao Zheng](mailto:yao.zheng@hawaii.edu) | Office Hours: see [here](../../../#contact) |

- **Format**:
| Lecture Time      | Lecture Location                             | Textbook                                                                            | Assignment | Project |
| ----               | ---                                         | ---                                                                                 | ---        | ---     |
| MW 13:30pm-14:45pm | [Zoom](https://hawaii.zoom.us/j/5764842348) | *Required*: Computer Architecture: A Quantitative Approach (5th Edition) (PH11)     | Individual | Team    |
|                    |                                             | *Optional*: Modern Processor Design: Fundamentals of Supperscalar Processors (SL13) |            |         |
|                    |                                             | *Optional*: FPGA Prototyping By Verilog Examples: Xilinx Spartan-3 Version          |            |         |

***
## Grading Policy
| ASSIGNMENTS | PROJECT | Discussion   | EXAM           |
| ----------  | ------  | ------------ | -------------- |
| 40%         | 40%     | 10%          | 10%            |

- **Cutoffs**
| A-     | B-    | C-    |
| ------ | ----- | ----- |
| 70%    | 50%   | 30%   |

- **Proscribed Conduct**: Copying or otherwise cheating on homework, lab reports, or exam will result in a failing grade for the course. More details can be found at student conduct code policies, [III.C.](http://studentaffairs.manoa.hawaii.edu/policies/conduct_code/proscribed_conduct.php)

***
## Schedule

| TIME                                                                 | TOPIC                                                  | LECTURE                                         | ASSIGNMENTS            | READING                                |
| ---------                                                            | ------------------------------------------------------ | ----------------------------------------------- | ---------------------- | -------------------------------------- |
| Week 01 ([Aug 25][recording 0825 url])                               | Introduction to Computer Architecture                  | [lec 01][lec 01 url]                            | --                     | PH11: Chapter 1, C1-C16.               |
| Week 02 ([Aug 30][recording 0830 url], [Sep 01][recording 0901 url]) | Review: Pipeline                                       | [lec 02][lec 02 url]                            | --                     | PH11: C26, C30-C58, C61-C81.           |
| Week 03 (Sep 08)                                                     | Review: Cache                                          | [lec 03][lec 03 url]                            | [assg 01][lab 01 url]  | PH11: B1-B40, SL13:177-209.            |
| Week 04 (Sep 13, Sep 15)                                             | Out-of-Order Processors                                | [lec 04a][lec 04a url] [lec 04b][lec 04b url]   | --                     | PH11:C43-C61, SL13:217-236.            |
| Week 05 (Sep 20, Sep 22)                                             | Branch, Register Renaming, and Memory Disambiguation   | [lec 05][lec 05 url]                            | --                     | SL13:237-273.                          |
| Week 06 (Sep 27, Sep 29)                                             | VLIW Introduction                                      | [lec 06][lec 06 url]                            | --                     | PH11: 192-196, Appendix H              |
| Week 07 (Oct 04, Oct 06)                                             | Branch Prediction, Advanced Cache Optimizations        | [lec 07a][lec 07a url] [lec 07b][lec 07b url]   | --                     | PH11: C26-C30, SL13:219-237, 453-508   |
| Week 08 (Oct 13)                                                     | Memory Protection                                      | [lec 08][lec 08 url]                            | [assg 02][lab 02 url]  | PH11:B41,B67,105-144                   |
| Week 09 (Oct 18, Oct 20)                                             | Vector Processors and GPUs                             | [lec 09a][lec 09a url] [lec 09b][lec 09b url]   | --                     | PH11:344-412                           |
| Week 10 (Oct 25, Oct 27)                                             | Course Project (Preliminary Presentations)             |                                                 | --                     | --                                     |
| Week 11 (Nov 01, Nov 03)                                             | Multithreading                                         | [lec 10][lec 10 url]                            | --                     | PH11:221-259                           |
| Week 12 (Nov 08, Nov 10)                                             | Parallel Programming and Small Multiprocessors         | [lec 11][lec 11 url]                            | --                     | PH11:386-400, 343-378                  |
| Week 13 (Nov 15, Nov 17)                                             | Interconnection Network                                | [lec 12][lec 12 url]                            | --                     | PH11:Appendix F                        |
| Week 14 (Nov 22, Nov 24)                                             | Large Multiprocessors (Directory Protocols)            | [lec 13][lec 13 url]                            | --                     | PH11:378-386, 400-429                  |
| Week 15 (Nov 29, Dec 01)                                             | Case Study: Software Define Radio Part 1               | [lec 14][lec 14 url]                            | --                     | --                                     |
| Week 16 (Dec 06, Dec 08)                                             | Case Study: Software Define Radio Part 2               | [lec 15][lec 15 url]                            | --                     | --                                     |
| Week 17                                                              | Course Project (Final Presentations)                   | --                                              | --                     | --                                     |

[recording urls]: # (recording urls)
[recording 0825 url]: https://youtu.be/mWXFyRLh4P8
[recording 0830 url]: https://youtu.be/cLpoRqQgGaY
[recording 0901 url]: https://youtu.be/j_hOQ5RBcsU

[lec urls]: # (lec urls)
[lec 01 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_01_slides.pdf
[lec 02 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_02_slides.pdf
[lec 03 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_03_slides.pdf
[lec 04a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_04_slides_a.pdf
[lec 04b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_04_slides_b.pdf
[lec 05 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_05_slides.pdf
[lec 06 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_06_slides.pdf
[lec 07a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_07_slides_a.pdf
[lec 07b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_07_slides_b.pdf
[lec 08 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_08_slides.pdf
[lec 09a url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_09_slides_a.pdf
[lec 09b url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_09_slides_b.pdf
[lec 10 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_11_slides.pdf
[lec 11 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_12_slides.pdf
[lec 12 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_13_slides.pdf
[lec 13 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_14_slides.pdf
[lec 14 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_15_slides_a.pdf
[lec 15 url]: https://s3-us-west-2.amazonaws.com/gustybear-websites/course_ee660_2021_fall/slides/ee660_2021_fall_materials_week_15_slides_b.pdf

[lab urls]: # (lab urls)
[lab 01 url]: ./laboratories/01/
[lab 02 url]: ./laboratories/02/
[lab 03 url]: # (tbd)

