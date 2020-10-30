---
draft: true
title: "Harmonic Radar for Monitoring of Coconut Rhinoceros Beetle"

subtitle: "Fall, 2020"

summary: "This project focuses on the design and implementation of a harmonic radar system to track the invasive Coconut Rhinoceros Beetle (CRB)."

tags:
- eex96
- harmonic radar
- sdr
- gnu radio
- cw radar
- passive transponder
- insect tracking

date: 2020-08-29T00:00:00-10:00

authors:
- Samson Aggelopoulos
- Willy Chang
- Brian Lu
- Matthew Sahara
- Yao Zheng

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, place an image named `featured.jpg/png` in your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
# Set `preview_only` to `true` to just use the image for thumbnails.
image:
  placement: 3
  caption: "Model ROBin with a semideterministic wiretap channel model"
  focal_point: "Center"
  preview_only: true
  alt_text: " "

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_pdf: ""
url_slides: ""
url_poster: ""
url_code: ""

# Markdown Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# Gallery
gallery_item:
  - album: images
    image: '05_IMG_3700.JPG'
    caption: 'Group performing on-site experiment (01).'

gallery_item:
  - album: images
    image: '06_IMG_3708.JPG'
    caption: 'Group performing on-site experiment (02).'

gallery_item:
  - album: images
    image: '07_IMG_3705.JPG'
    caption: 'Group performing on-site experiment (03).'

gallery_item:
  - album: images
    image: '08_IMG_3702.JPG'
    caption: 'Group performing on-site experiment (04).'

gallery_item:
  - album: images
    image: '01_semideterministic_wiretap.JPG'
    caption: 'The security of channel randomized orthogonal blinding
    can be analyzed via a Semideterministic wiretap channel model.'

gallery_item:
  - album: images
    image: '02_rotating_antenna.JPG'
    caption: 'Rotating Antenna to achieve channel randomization.'

gallery_item:
  - album: images
    image: '04_setup_2020_03_05.png'
    caption: 'Experiment setup for 2020/03/05.'

---

## Problem Statement
The Coconut Rhinoceros Beetle (CRB) is an invasive insect originating from Southeast Asia. The appearance of these beetles in tropical locations present a grave threat to local ecosystems. According to the [USDA](https://www.aphis.usda.gov/aphis/resources/pests-diseases/hungry-pests/the-threat/coconut-rhinoceros-beetle/hp-crp), the CRB raises concerns specifically in Hawaii, Guam, and American Samoa. CRBs are known to harm a variety of fibrous plants, such as coconut trees, pineapple and sugarcane. The State of Hawaii has taken measures to capture and control the invasion of the CRB using panel traps suspended from trees throughout the islands. Our project focuses on tracking the behavior of these beetles in controlled areas in Guam.

Tracking the CRB is essential to unveil key behavioral information, such as foraging and breeding habits in adult beetles.

## Proposed Solution
We are designing a radar system to track individual CRBs. Harmonic radar is commonly used to track insects to better understand behavioral characteristics.

There are two parts to harmonic radar: 1) Base station handling the transmit (Tx) and receive (Rx) aspects of our radar system and 2) Transponders mounted on individual CRBs.



***

## Gallery

{{< gallery album="images" >}}

Up to down, left to right: semideterministic wiretap channel model, rotating antenna to achieve channel randomization. experiment setups. On-site experiments.

***

## Project Specifications
### SDR
- GNU Radio
  - USRP node: Ettus N210 @ 10.10.3.10
  - Rotator: Calypso @ 10.10.3.133
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
RF Transponder
- Testing antenna designs:
  - Bowtie (printed dipole)
  - J-Pole
  - Wire (with printed line)
-
