---
title: "Wireless and Cybersecurity Laboratory (WCL)"
date: "2018-05-03T18:13:12-10:00"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags:
- facility
- wireless
- security
- sensor
- communication
- radar
- mmwave
- sensor

authors:
- Yao Zheng

summary: "WCL is a 400 sq ft space located at the fourth floor of Holmes Hall, curating a selection of RF instruments for wireless research and development."

# Featured image
# To use, place an image named `featured.jpg/png` in your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
# Set `preview_only` to `true` to just use the image for thumbnails.
image:
  placement: 3
  caption: ""
  focal_point: "Center"
  preview_only: true
  alt_text: " "

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

gallery_item:
 - album: laboratory
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0191.JPG
   caption: Testing and fabrication bench
 - album: laboratory
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0192.JPG
   caption: RF development bench
 - album: laboratory
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0193.JPG
   caption: Break area
 - album: laboratory
   image: https://github.com/gustybear-research/facility/raw/main/gallery/_DSC2091_00002.jpg
   caption: Student activities 1
 - album: laboratory
   image: https://github.com/gustybear-research/facility/raw/main/gallery/_DSC2171_00011.jpg
   caption: Student activities 2

 - album: rf_research
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0185.JPG
   caption: Custom mmWave comm/sensing/sounder system
 - album: rf_research
   image: https://github.com/gustybear-research/facility/raw/main/gallery/_DSC2082_00001.jpeg
   caption: TMYTEK BBox Lites mmWave phased array
 - album: rf_research
   image: https://github.com/gustybear-research/facility/raw/main/gallery/phased-array-antenna-structure.png
   caption: TMYTEK BBox Lites mmWave phased array model
 - album: rf_research
   image: https://github.com/gustybear-research/facility/raw/main/gallery/phasedarray-radiation-pattern.png
   caption: TMYTEK BBox Lites mmWave phased array pattern
 - album: rf_research
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0188.JPG
   caption: Wi-Fi sensing system
 - album: rf_research
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0189.JPG
   caption: Rotating middle band antenna

 - album: instruments and fabrication
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0190.JPG
   caption: Keysight N9918A
 - album: instruments and fabrication
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0187.JPG
   caption: Keysight N9010B
 - album: instruments and fabrication
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0181.JPG
   caption: Keysight 33210A
 - album: instruments and fabrication
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0186.JPG
   caption: Keysight DSOX1102G
 - album: instruments and fabrication
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0182.JPG
   caption: Keysight E36313A
 - album: instruments and fabrication
   image: https://github.com/gustybear-research/facility/raw/main/gallery/IMG_0183.JPG
   caption: Fluke 45

 - album: acknowledgement
   image: https://github.com/gustybear-research/facility/raw/main/sponsor/keysight-logo.png
   caption: Keysight
 - album: acknowledgement
   image: https://github.com/gustybear-research/facility/raw/main/sponsor/niLogo.png
   caption: NI
 - album: acknowledgement
   image: https://github.com/gustybear-research/facility/raw/main/sponsor/TMY-logo-01.png
   caption: TMYTEK
---
***

# Executive Summary

This laboratory in Holmes Hall 488 is used for experimental work involving radio frequency (RF) communication, sensing, and security. The laboratory provides RF prototyping equipment and instruments, including mmWave beamforming kit, software-defined radios (SDRs), signal generators, spectrum analyzers, network analyzers; fabrication and assembly tools, including soldering and reworking stations, RF components, including cables, attenuators, power splitters/combiners, directional couplers; design and simulation software for ICs and PCBs; and other miscellaneous. The laboratory provides project participants with private server clusters, laptops, and desktop computers; various software licenses, including MATLAB, Candence, LabVIEW, OriginLab, and Adobe Creative Cloud; and remote access to all instruments, computers, and actuators.

{{< gallery-enhance album="laboratory" numbered="true" caption="Laboratory Overview">}}

***
# Logistics
| Location        | Physical Access                                                                                                              | Remote Access                                   |
| ----            | ---                                                                                                                          | ---                                             |
| Holmes Hall 488 | contact [EE office](mailto:eeoffice@hawaii.edu) | contact [Yao Zheng](mailto:yaozheng@hawaii.edu) |

***

# Resource

## RF Research and Prototype
{{< gallery-enhance album="rf_research" numbered="true" caption="RF Research and Prototype">}}

- **mmWave Comm/Sensing/Sounder**: The customized 24-31GHz radio system implemented with a mmWave beamforming kit (BBox Lites/UD Box from TMYTEK), Ettus USRPs (N210, CDA-2990), and COTS Wi-Fi NICs (Intel 5300). The system consists of a 16-channel 24-31GHz phased array antenna and a frequency Up/Down converter, which interfaces with baseband devices (LabVIEW controlled USRPs or COTS Wi-Fi NICs). Each channel provides $ 360^{\circ} $ phase shifter coverage with $ 5^{\circ} $ per step, 400 ms beam switching time. The 3dB beam aperture is $ 13^{\circ} $ horizontally and $ 14^{\circ} $ vertically. The angle coverage is +/-$ 45^{\circ} $ horizontally and +/-$ 60^{\circ} $ vertically. The baseband devices can support up to 80MHz bandwidth with 64 subcarriers for data transmission or CSI measurements.

- **Ansys HFSS**: HFSS is a commercial finite element method solver for electromagnetic structures from Ansys. The acronym stands for high-frequency structure simulator. HFSS is one of several commercial tools used for antenna design, and the design of complex radio frequency electronic circuit elements including filters, transmission lines, and packaging.

## Instruments and Fabrications

{{< gallery-enhance album="instruments and fabrication" numbered="true" caption="Instruments and Fabrications">}}

- **Spectrum Analyzers (Keysight N9010B, N9918A)**: The benchtop model (Keysight N9010B) operates from 10Hz to 7GHz and is upgraded with a pre-amplifier and 40MHz analysis bandwidth. The handheld model (Keysight N9918A) operates from 30kHz to 26.5GHz and is upgraded with vector network analysis functions.
- **Signal Generators (Keysight 33210A)**: One basic signal generator for primary waveforms and 8K points of complex arbitrary waveforms.
- **Oscilloscopes (Keysight DSOX1102G)**: One basic oscilloscope operates up to
    100 MHz, 50,000 wfms/sec update rate.
- **Power Supplies (Keysight E36313A)**: One low noise power supply (ripple and
    noise $ < $ 350 $\mu$Vrms) with 4-wire sense to improve measurement accuracy.
- **Multimeter (Fluke 45)**: One basic digital multimeter with dual display,
    standard rs-232c interface, and dB measurement.

# Acknowledgement

{{< gallery-enhance album="acknowledgement" numbered="true" caption="acknowledgement and sponsors">}}

The laboratory is developed with the generous support from
[Keysight](https://www.keysight.com/us/en/home.html),
[NI](https://www.ni.com/en-us.html), and [TMYTEK](https://www.tmytek.com/).
***
