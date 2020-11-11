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
- Marionne Casipit
- Mark Kwon 
- Will Bracken
- Samson Aggelopoulos
- Willy Chang
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
#{{< gallery album="images" >}}

---
## Abstract
Wireless physical layer security scheme, such as orthogonal blinding, is able to achieve this level of secure communications by transmitting artificial noise into the null-space of the receiver's channel, thus corrupting reception of any unwanted eavesdroppers.  This physical-layering method supersedes other theoretical methods, such as zero-forcing beam-forming because it does not rely on having any prior knowledge about an eavesdroppers channel.  Security based analysis supports the idea that Orthogonal blinding can closely approach the same secrecy rate as zero-force beam-forming when compared to single-antenna eavesdroppers.  However, further analysis shows that orthogonal blinding is less effective against multi-antenna eavesdroppers.  This is because multi-antenna eavesdroppers would have sufficient spatial dimensions to aid them in separating the original message from the artificial generated noise. Schulz and Zheng et al. demonstrates that an eavesdropper can leverage a known or low entropy symbols in a transmission and quickly create a decoding filter in order to recover the missing pieces of the transmission; equivalent to a known-plaintext attack in crypto-analysis.  In this project, we investigate an orthogonal blinding based physical-layer security method immune to the known-plaintext attack.
***

## Gallery
### Project Activities

### Methodology

### System Design

### Implemetations

### Experiments


Up to down, left to right: semideterministic wiretap channel model, rotating antenna to achieve channel randomization. experiment setups. On-site experiments.

***

## Project Description

### Background

### Methodology

### System Design

### Implementations

### Experiments
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

#### Data (2020/01/23)
| Scenario | Alice Gain[^1] | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotation Speed (rpm)[^2] | Time (s) | Data                   |
| ---      | ---            | ---      | ---      | ---                    | ---      | ---                      | ---      | ---                    |
| 01       | 30dB           | 0dB      | 0dB      | 1.6G                   | 500k     | 3                        | 100      | [Download][s01_1_6G_a] |
| 01       | 45dB           | 0dB      | 0dB      | 1.6G                   | 500k     | 3                        | 100      | [Download][s01_1_6G_b] |
| 01       | 60dB           | 0dB      | 0dB      | 1.6G                   | 500k     | 3                        | 100      | [Download][s01_1_6G_c] |
| 01       | 30dB           | 0dB      | 0dB      | 2.6G                   | 500k     | 3                        | 100      | [Download][s01_2_6G_a] |
| 01       | 45dB           | 0dB      | 0dB      | 2.6G                   | 500k     | 3                        | 100      | [Download][s01_2_6G_b] |
| 01       | 60dB           | 0dB      | 0dB      | 2.6G                   | 500k     | 3                        | 100      | [Download][s01_2_6G_c] |
| 01       | 45dB           | 0dB      | 0dB      | 3.6G                   | 500k     | 3                        | 100      | [Download][s01_3_6G_a] |
| 01       | 60dB           | 0dB      | 0dB      | 3.6G                   | 500k     | 3                        | 100      | [Download][s01_3_6G_b] |

#### Data (2020/01/23)
| Scenario | Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotation Speed (rpm) | Time (s) | Data                   |
| ---      | ---        | ---      | ---      | ---                    | ---      | ---                  | ---      | ---                    |
| 02       | 30dB       | 0dB      | 0dB      | 0.9G                   | 500k     | 3                    | 100      | [Download][s02_0_9G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 0.9G                   | 500k     | 3                    | 100      | [Download][s02_0_9G_b] |
| 02       | 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | 3                    | 100      | [Download][s02_1_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 1.6G                   | 500k     | 3                    | 100      | [Download][s02_1_6G_b] |
| 02       | 30dB       | 0dB      | 0dB      | 2.6G                   | 500k     | 3                    | 100      | [Download][s02_2_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 2.6G                   | 500k     | 3                    | 100      | [Download][s02_2_6G_b] |
| 02       | 30dB       | 0dB      | 0dB      | 3.6G                   | 500k     | 3                    | 100      | [Download][s01_3_6G_a] |
| 02       | 45dB       | 0dB      | 0dB      | 3.6G                   | 500k     | 3                    | 100      | [Download][s01_3_6G_b] |

#### Data (2020/03/05)

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Reflector | Rot. Speed (rpm) | Time (s) | Data                    |
| ---            | ---      | ---      | ---                    | ---      | ---       | ---                  | ---      | ---                     |
| 30dB           | 0dB      | 0dB      | 1.6G                   | 500k     | small     | 3                    | 100      | [Download][20200305tx1] |
| 30dB           | 0dB      | 0dB      | 1.6G                   | 500k     | large     | 3                    | 100      | [Download][20200305tx2] |
| 45dB           | 0dB      | 0dB      | 2.6G                   | 500k     | small     | 3                    | 100      | [Download][20200305tx3] |
| 45dB           | 0dB      | 0dB      | 2.6G                   | 500k     | large     | 3                    | 100      | [Download][20200305tx4] |
| 60dB           | 0dB      | 0dB      | 3.6G                   | 500k     | small     | 3                    | 100      | [Download][20200305tx5] |
| 60dB           | 0dB      | 0dB      | 3.6G                   | 500k     | large     | 3                    | 100      | [Download][20200305tx6] |

#### Data (2020/09/10)

| Alice (High Gain) Gain | Bob (Rotator) Gain | Central Frequency (Hz) | I/Q Rate | Configuration  | Rot. Speed (rpm) | Time (s) | Data                    |
| ---                    | ---                | ---                    | ---      | ---            | ---              | ---      | ---                     |
| 30dB                   | 10dB                | 2.4G                   | 500k     | 1 LOS          | 3                | 100      | [Download][20200910tx1] |
| 15dB                   | 10dB                | 2.4G                   | 500k     | 1 LOS          | 3                | 100      | [Download][20200910tx2] |
| 30dB                   | 10dB                | 2.4G                   | 500k     | 1 LOS          | 1                | 100      | [Download][20200910tx3] |
| 30dB                   | 10dB                | 2.4G                   | 500k     | 2 LOS          | 3                | 100      | [Download][20200910tx4] |
| 15dB                   | 10dB                | 2.4G                   | 500k     | 2 LOS          | 3                | 100      | [Download][20200910tx5] |
| 30dB                   | 10dB                | 2.4G                   | 500k     | 2 LOS          | 1                | 100      | [Download][20200910tx6] |
| 30dB                   | 10dB                | 2.4G                   | 500k     | 1 LOS + 1 NLOS | 3                | 100      | [Download][20200910tx7] |
| 15dB                   | 10dB                | 2.4G                   | 500k     | 1 LOS + 1 NLOS | 3                | 100      | [Download][20200910tx8] |
| 30dB                   | 10dB                | 2.4G                   | 500k     | 1 LOS + 1 NLOS | 1                | 100      | [Download][20200910tx9] |

[data url]: # (week urls)
[20200305tx1]: https://drive.google.com/drive/folders/18HvVHh6jX6pAW3hYXT5nDg1-sqBfGj48?usp=sharing
[20200305tx2]: https://drive.google.com/drive/folders/1nhf3eIN3QANTaydRQtuBElWAtWEqaz6r?usp=sharing
[20200305tx3]: https://drive.google.com/drive/folders/1616RRzrZKQKsaccJE-9oIBQ6WA4RHc9a?usp=sharing
[20200305tx4]: https://drive.google.com/drive/folders/1OzVybveZ_WCEPkBpp4MXDyA8_7H0hzEo?usp=sharing
[20200305tx5]: https://drive.google.com/drive/folders/1wOFwO2q2H1nj1vKa5nug3C6dhkmeh9zv?usp=sharing
[20200305tx6]: https://drive.google.com/drive/folders/15UYoHH5UFcwrdzKSBMtddNZqKAAjIEMy?usp=sharing

[data url]: # (week urls)
[20200910tx1]: https://drive.google.com/drive/folders/1DukCFhMV0JIaa_o-JSbRuNfPKtjXCBM8?usp=sharing
[20200910tx2]: https://drive.google.com/drive/folders/1YeljUP8lWL5bPzJAiDs2IrC9TP0GaMv2?usp=sharing
[20200910tx3]: https://drive.google.com/drive/folders/1k82Tl91oFaoKzvHKht5OIsUcp4kVORGS?usp=sharing
[20200910tx4]: https://drive.google.com/drive/folders/1UuMLyeA7oqbhLyYeNpjKn-BvdtyjOk2x?usp=sharing
[20200910tx5]: https://drive.google.com/drive/folders/1X2TXBeKLtwyGM8LlsTcVOHueIBHSvu13?usp=sharing
[20200910tx6]: https://drive.google.com/drive/folders/1CqN_vBd9r29aui4zJ1CLoC7hs2zXr68s?usp=sharing
[20200910tx7]: https://drive.google.com/drive/folders/1rXJyat7lq60lceV6__Mzy7dLEkZx9AQU?usp=sharing
[20200910tx8]: https://drive.google.com/drive/folders/1SGVuYgjHHKMY_dYCCFcbdg-cWKMYdgCa?usp=sharing
[20200910tx9]: https://drive.google.com/drive/folders/1s_A9GRoWq0ZNEKlnmPxttWlso84oX0Ls?usp=sharing

[^1]: The rotating speed is based on actual measurment instead of the input
  value to the rotator interface. For instance, the actual rotating speed is 3rpm when  the input value is 10rpm.

[^2]: The gain range of the SBX daughter board used by the experiment is 0.0
  to 31.5 dB step 0.5dB. Therefore, to set the gain to 9dB in Labview, the gain step should be 18. The WAT5VJB LPA gives approxmiately 10 dBi gain in its boom direction.
