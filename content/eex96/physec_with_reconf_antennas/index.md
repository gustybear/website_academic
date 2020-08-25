---
title: "Enhancing Orthogonal Blinding with Channel Randomization"
subtitle: "Spring, 2020"
date: 2020-01-10T00:00:00-10:00
authors: ["Will Bracken", "Marionne Casipit", "Mark Kwon", "Yao Zheng"]
tags: ["eex96", "wireless", "SDR", "current", "featured"]

abstract: 'This project implements ROBin: Channel Randomizing Orthogonal Blinding, an enhanced wireless physical layer security scheme robust to known-plaintext attack.'

# Featured image
# To use, place an image named `featured.jpg/png` in your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
# Set `preview_only` to `true` to just use the image for thumbnails.
image:
  placement: 3
  caption: " "
  focal_point: "Center"
  preview_only: true
  alt_text: " "

gallery_item:
  - album: images
    image: 'scenario_01.png'
    caption: 'Scenario 01'

gallery_item:
  - album: images
    image: 'scenario_02.png'
    caption: 'Scenario 02'
---
***
## Abstract
Wireless physical layer security scheme, such as orthogonal blinding, is able to achieve this level of secure communications by transmitting artificial noise into the null-space of the receiver's channel, thus corrupting reception of any unwanted eavesdroppers.  This physical-layering method supersedes other theoretical methods, such as zero-forcing beam-forming because it does not rely on having any prior knowledge about an eavesdroppers channel.  Security based analysis supports the idea that Orthogonal blinding can closely approach the same secrecy rate as zero-force beam-forming when compared to single-antenna eavesdroppers.  However, further analysis shows that orthogonal blinding is less effective against multi-antenna eavesdroppers.  This is because multi-antenna eavesdroppers would have sufficient spatial dimensions to aid them in separating the original message from the artificial generated noise. Schulz and Zheng et al. demonstrates that an eavesdropper can leverage a known or low entropy symbols in a transmission and quickly create a decoding filter in order to recover the missing pieces of the transmission; equivalent to a known-plaintext attack in crypto-analysis.  In this project, we investigate an orthogonal blinding based physical-layer security method immune to the known-plaintext attack.
***

## Gallary

{{< gallery album="images" >}}
Left to right: Scenario 01, Scenario 02.

## Experiments
### Equipment
- Alice
  - USRP node: Ettus N210 @ 10.10.3.10
  - Rotator: Calypso @ 10.10.3.133
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Bob
  - USRP node: Ettus N210 @ 10.10.3.25
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Eve
  - USRP node: Ettus N210 @ 10.10.3.20;10.10.3.15
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)

### Scenario 01

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---     | ---                      | ---      | ---                              |
| 30dB[^2]   | 0dB      | 0dB      | 2.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 01a][scenario 01a url] |
| 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 01b][scenario 01b url] |
| 30dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 01c][scenario 01c url] |

### Scenario 02

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---     | ---                      | ---      | ---                              |
| 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 02b][scenario 02b url] |
| 45dB       | 0dB      | 0dB      | 2.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 02a][scenario 02a url] |
| 60dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 02c][scenario 02c url] |

***
## Demonstrations

[data url]: # (week urls)
[scenario 01a url]: # ()
[scenario 01b url]: # ()
[scenario 01c url]: # ()
[scenario 01d url]: # ()
[scenario 01e url]: # ()
[scenario 01f url]: # ()
[scenario 01g url]: # ()
[scenario 01h url]: # ()

[scenario 02a url]: # ()
[scenario 02b url]: # ()
[scenario 02c url]: # ()
[scenario 02d url]: # ()
[scenario 02e url]: # ()
[scenario 02f url]: # ()
[scenario 02g url]: # ()
[scenario 02h url]: # ()

[^1]: The rotating speed is based on actual measurment instead of the input
  value to the rotator interface. For instance, the actual rotating speed is 3rpm when  the input value is 10rpm.

[^2]: The gain range of the SBX daughter board used by the experiment is 0.0
  to 31.5 dB step 0.5dB. Therefore, to set the gain to 9dB in Labview, the gain step should be 18. The WAT5VJB LPA gives approxmiately 10 dBi gain in its boom direction.
