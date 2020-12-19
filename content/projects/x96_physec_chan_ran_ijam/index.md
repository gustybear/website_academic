---
draft: true
title: "Enhancing Wireless Physcial-Layer Security with Channel Randomization"

subtitle: "Spring, 2020"

summary: "This project implements Channel Randomizing Orthogonal Blinding, an enhanced wireless physical-layer security scheme robust to eavesdropper with multiple antennas."

tags:
- eex96
- physical layer security
- channel randomization
- reconfigurable antenna
- iJam
- labview
- sdr
- current
- featured

date: 2020-01-10T00:00:00-10:00

authors:
- Samson Aggelopoulos
- Willy Chang
- Maile Kennaugh
- Brian Lu
- Matthew Sahara
- Alvin Yang
- Thomas Yang
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
# gallery_item:
#   - album: images
#     image: '05_IMG_3700.JPG'
#     caption: 'Group performing on-site experiment (01).'
#
# gallery_item:
#   - album: images
#     image: '06_IMG_3708.JPG'
#     caption: 'Group performing on-site experiment (02).'
#
# gallery_item:
#   - album: images
#     image: '07_IMG_3705.JPG'
#     caption: 'Group performing on-site experiment (03).'
#
# gallery_item:
#   - album: images
#     image: '08_IMG_3702.JPG'
#     caption: 'Group performing on-site experiment (04).'
#
#
# gallery_item:
#   - album: images
#     image: '02_rotating_antenna.JPG'
#     caption: 'Rotating Antenna to achieve channel randomization.'
#
# gallery_item:
#   - album: images
#     image: '04_setup_2020_03_05.png'
#     caption: 'Experiment setup for 2020/03/05.'
#
# gallery_item:
#   - album: images
#     image: '13_DSC_0247.JPG'
#     caption: 'Experiment setup for 2020/09/10.'
#
# gallery_item:
#   - album: images
#     image: '10_DSC_0238.JPG'
#     caption: 'Experiment setup for 2020/09/10.'
#
# gallery_item:
#   - album: images
#     image: '11_DSC_0243.JPG'
#     caption: 'Experiment setup for 2020/09/10.'
#
# gallery_item:
#   - album: images
#     image: '12_DSC_0245.JPG'
#     caption: 'Experiment setup for 2020/09/10.'
#
# gallery_item:
#   - album: images
#     image: '14_DSC_0244.JPG'
#     caption: 'Experiment setup for 2020/09/10.'
gallery_item:
 - album: gallery
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/DSC_0239.jpg
   caption: Experimental setup with two high gain antennas and a rotating antenna.
 - album: gallery
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/DSC_0243.jpg
   caption: Experimental setup with two high gain antennas and a rotating antenna.
 - album: gallery
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/DSC_0246.jpg
   caption: Closeup of the high gain antenna.
 - album: gallery
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/DSC_0248.jpg
   caption: Closeup of the rotating antenna.
 - album: gallery
   image:  https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/DSC_0249.jpg
   caption: Matthew holding a planarly reflector.
 - album: gallery
   image:  https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/IMG_3668.jpg
   caption: Experiment with corner reflectors.
 - album: gallery
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/IMG_3706.jpg
   caption: Interfacing with the software used in the experiment.
 - album: gallery
   image:  https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/IMG_3702.jpg
   caption: Team picture!

---
***
{{< gallery >}}
## Abstract
Wireless physical layer security scheme, such as orthogonal blinding, is able to achieve this level of secure communications by transmitting artificial noise into the null-space of the receiver's channel, thus corrupting reception of any unwanted eavesdroppers.  This physical-layering method supersedes other theoretical methods, such as zero-forcing beam-forming because it does not rely on having any prior knowledge about an eavesdroppers channel.  Security based analysis supports the idea that Orthogonal blinding can closely approach the same secrecy rate as zero-force beam-forming when compared to single-antenna eavesdroppers.  However, further analysis shows that orthogonal blinding is less effective against multi-antenna eavesdroppers.  This is because multi-antenna eavesdroppers would have sufficient spatial dimensions to aid them in separating the original message from the artificial generated noise. Schulz and Zheng et al. demonstrates that an eavesdropper can leverage a known or low entropy symbols in a transmission and quickly create a decoding filter in order to recover the missing pieces of the transmission; equivalent to a known-plaintext attack in crypto-analysis.  In this project, we investigate an orthogonal blinding based physical-layer security method immune to the known-plaintext attack.

***

## Highlights
Select up to five figures to display in project highlights

***
## Acknowledgement
This project is partially supported NSF grants CNS-1948568, CNS-1948568, and
TMYTEK mmWave research initiative.

***

## Description

### Introduction
Thomas


### Background
Brian
### Methodology

### Implementation and Experimentation

### Conclusion
Sampson
#### Equipment
- Alice
  - USRP node: Ettus N210
  - Antenna(s)[decimeter ban]: WAT5VJB log-periodic (850-6500 MHz)
  - Antenna(s)[mmWave band]: TMYTEK BBox Lite (24000 - 30000 MHz)
- Bob
  - USRP node: Ettus N210
  - Antenna(s)[decimeter band): WAT5VJB or PE51082 (2400 MHz only)
  - Antenna(s)[mmWave band]: TMYTEK BBox Lite (24000 - 30000 MHz)
- Eve
  - USRP node: Ettus N210
  - Antenna(s)[decimeter band): WAT5VJB or PE51082 (2400 MHz only)
  - Antenna(s)[mmWave band]: TMYTEK BBox Lite (24000 - 30000 MHz)
- RF reflector
  - Large corner, small corner, plane reflector.

#### Procedure
***

## Figures

***

## Data Archive
#### Exp. 2020/01/23
| Scenario | Alice Gain[^1] | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Reflector    | Rot. Speed (rpm)[^2] | Time (s) | Data                   |
| ---      | ---            | ---      | ---      | ---                    | ---      | ---          | ---                  | ---      | ---                    |
| 01       | 30dB           | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_1_6G_a] |
| 01       | 45dB           | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_1_6G_b] |
| 01       | 60dB           | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_1_6G_c] |
| 01       | 30dB           | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_2_6G_a] |
| 01       | 45dB           | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_2_6G_b] |
| 01       | 60dB           | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_2_6G_c] |
| 01       | 45dB           | 0dB      | 0dB      | 3.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_3_6G_a] |
| 01       | 60dB           | 0dB      | 0dB      | 3.6G                   | 500k     | Corner (lg) | 3                    | 100      | [Download][s01_3_6G_b] |

#### Exp. 2020/01/30
| Scenario | Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Reflector   | Rot. Speed (rpm) | Time (s) | Data                   |
| ---      | ---        | ---      | ---      | ---                    | ---      | ---         | ---              | ---      | ---                    |
| 02       | 30dB       | 0dB      | 0dB      | 0.9G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_0_9G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 0.9G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_0_9G_b] |
| 02       | 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_1_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_1_6G_b] |
| 02       | 30dB       | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_2_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_2_6G_b] |
| 02       | 30dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s01_3_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s01_3_6G_b] |

#### Exp. 2020/03/05
| Scenario | Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Reflector   | Rot. Speed (rpm) | Time (s) | Data                   |
| ---      | ---        | ---      | ---      | ---                    | ---      | ---         | ---              | ---      | ---                    |
| 02       | 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (sl) | 3                | 100      | [Download][s02_1_6G_a] |
| 02       | 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_1_6G_b] |
| 02       | 45dB       | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (sl) | 3                | 100      | [Download][s02_2_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 2.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_2_6G_b] |
| 02       | 60dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Corner (sl) | 3                | 100      | [Download][s02_3_6G_a] |
| 02       | 60dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Corner (lg) | 3                | 100      | [Download][s02_3_6G_b] |

#### Exp. 2020/09/10

| Scenario | Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Reflector | Rot. Speed (rpm) | Time (s) | Data                   |
| ---      | ---        | ---      | ---      | ---                    | ---      | ---       | ---              | ---      | ---                    |
| 03       | 15dB       | 0dB      | NA       | 2.4G                   | 500k     | NA        | 3                | 100      | [Download][s03_2_4G_a] |
| 03       | 30dB       | 0dB      | NA       | 2.4G                   | 500k     | NA        | 3                | 100      | [Download][s03_2_4G_b] |
| 03       | 30dB       | 0dB      | NA       | 2.4G                   | 500k     | NA        | 1                | 100      | [Download][s03_2_4G_c] |
| 04       | 15dB       | 0dB      | NA       | 2.4G                   | 500k     | NA        | 3                | 100      | [Download][s04_2_4G_a] |
| 04       | 30dB       | 0dB      | NA       | 2.4G                   | 500k     | NA        | 3                | 100      | [Download][s04_2_4G_b] |
| 04       | 30dB       | 0dB      | NA       | 2.4G                   | 500k     | NA        | 1                | 100      | [Download][s04_2_4G_c] |
| 05       | 15dB       | 0dB      | NA       | 2.4G                   | 500k     | Plane     | 3                | 100      | [Download][s05_2_4G_a] |
| 05       | 30dB       | 0dB      | NA       | 2.4G                   | 500k     | Plane     | 3                | 100      | [Download][s05_2_4G_b] |
| 05       | 30dB       | 0dB      | NA       | 2.4G                   | 500k     | Plane     | 1                | 100      | [Download][s05_2_4G_c] |

[data url]: # (week urls)

[^1]: The rotating speed is based on actual measurment instead of the input
  value to the rotator interface. For instance, the actual rotating speed is 3rpm when  the input value is 10rpm.

[^2]: The gain range of the SBX daughter board used by the experiment is 0.0
  to 31.5 dB step 0.5dB. Therefore, to set the gain to 9dB in Labview, the gain step should be 18. The WAT5VJB LPA gives approxmiately 10 dBi gain in its boom direction.
