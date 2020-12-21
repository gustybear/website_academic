---
draft: false
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
## Presentation
{{< youtube id="DPqoX8ZLRdo" >}}

***

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
(Thomas)
When performing RF communication between a transmitter and receiver, the signal observes a channel effect, which is dependent on many factors, such as scattering, fading, and power decay as the distance increases. This means the signal sent by the transmitter will not be the signal received by the receiver. However, it is possible to undo this channel effect on the signal with the use of pilot symbols. By utilizing a universal truth where everyone knows what value the pilot symbols are and their position in the message, we can calculate the channel effect by dividing the received pilot symbols by the original pilot symbols, and using this value to remove the channel effect on our received signal.

RF communication is unsecure however, as the tranmission is unencrypted and can easily be seen by an eavesdropper. To establish an encrypted communications channel, iJam, a key exchange protocol, was introduced such that a key can be exchanged over the RF channel. The iJam protocol requires the transmitter, Alice, to send each key symbol twice. The receiver, Bob, equipped with a second transmitting antenna, will randomly choose which key symbol to jam with his second antenna. Since Bob knows which of the two key symbols is being jammed, he can pick out the unjammed symbol, then reconstruct the key by accumulating the unjammed symbols. From an Eavesdropper, Eve's point of view, she is unsure which of the pair of key symbols is the jammed symbol and which is not, leading to a 50% chance of guessing which symbol is correct, effectively obscuring the key from others.

The downfall to iJam is that it only works against single-antenna eavesdropper. With a multi-antenna setup, an eavesdropper can use the additional spatial diversity, the pilot symbols used to calculate the channel effect, and the unchanging channel between the legitimate transmitter and itself to equalize the channel between itself and the transmitter determine which of the two symbols is being jammed, therefore picking out the unjammed symbols and reconstructing the key.

This is where we propose a defense mechanism against multi-antenna eavesdropper, iJam with channel randomization. This builds off of iJam and comes in two parts: precode the channel effect that we expect to see between the Alice and Bob, removing the need for pilot symbols, and to constantly rotate the transmitting antenna to create a constantly changing channel. In order to precode the channel effect, we develop a training model, or a angle-of-departure (AoD) estimation algorithm, to predict the channel effect, which is effective in a unchanging environment. Since we precode the channel effect on Alice's side, the receiving signal that Bob sees requires no further processing, and no longer needs pilot symbols to undo the channel effect. Since there are no longer any pilot symbols in the transmission, an eavesdropper can no longer calculate the channel effect between itself and Alice, thus unable to decipher the key symbols. As for the second part, we constantly rotate Alice's antenna, which in turn constantly changes the channel. In conjunction with the first part, our AoD estimation algorithm will be trained with the angles that we will use as we rotate, so we have a wide range of channels to use. We do this since in contrast, had we kept a constant channel by not rotating the antenna, an eavesdropper with enough time can decipher the channel effect and recover the key. By constantly changing the channel, an eavesdropper is unable to keep up and cannot determine the channel effect, securing the key transmission.

### Background
(Maile / Brian)
You're writing about iJam and how it works, channel state information, and how iJam is vulnerable to multi-antenna setups

### Methodology
(Willy) To predict the CSI for different antenna modes without sending the pilots symbols, Alice computes the angle of departure vector (AoD) using a subset of antenna modes dedicated for training. This can be modeled as follows:

$$\mathbf Y = \mathbf H\mathbf X + \mathbf N$$

where $\mathbf Y$ is the signals received by Bob, $\mathbf H$ is the channel state information (CSI), $\mathbf X$ is the transmitted signal Alice trasmits, and $\mathbf N$ is the channel noise.

$\mathbf H$ can be modeled as follows:

the inner product between the area of departure (AoD) vector, $\mathbf h$, and the transmitter's (TX) antenna pattern, $a$. This can be represented in the following equation:

$$\mathbf H = \sum a\mathbf h$$

Each element in the AoD vector $\mathbf h$ represents the environment's attentuation effect on the TX signal in a specific direction. Within a short period of time, these elements do not change.

To solve this model, the MUSIC (Multiple Signal Classification) algorithm is used to compute the AoD vector. This algorithm minizes the difference between the estimation and ground truth CSI. A regular MUSIC algorithm requires Alice to measure the CSI with a sufficient number of antenna modes during the training phase in order to solve for the AoD. However, this significantly limits the number of available antenna modes for data transmission.

To reduce the number of antenna modes used during training, and consequently increasing the number of antenna modes for data transmission, the problem is converted into a regularized underdetermined LP with less equations than the unknowns. This problem is then solved with a compressive sensing technique.

With the computed AoD, Alice will be able to predict $\mathbf H$ during transmission and sends the product of the inverse of $\mathbf H$ multiplied to $\mathbf X$ in order to pre-equalize the channel for Bob.

### Implementation and Experimentation
(Alvin)
iJam with Channel Randomization was implemented by connecting various hardware components with Labview, which allows us to interface with each hardware component in order to perform our experiments. The implementation and experimentation we will be going over in detail with be of the 09/10/2020 experiment.

The hardware used in this experiment are two high gain directional antennas (PE51082) for Bob and Eve, a rotating antenna (WAT5VJB) for Alice, a planar RF reflector, as well as USRPs (Ettus N210) for each antenna to generate and receive signals.
In Labview, we are able to have Alice transmit either a randomized bitstream or a bitstream with all ones, and we can then view the received signal at both Bob's and Eve's end. Channel randomization can then be toggled, by taking the channel effect at the receiver side, and precodes it to Alice's signal. As an angle of departure algorithm has not yet been implemented, a temporary solution was used where we take the channel state information at the receiver and use that to precode the message.

In the 09/10 experimentation, we ran with three scenarios. These scenarios are modeled in figures 1-3.

The various scenarios were picked in order to determine whether we can view the reflected signal path when running the experiment, to verify that we are processing/receiving the data correctly. Along with this, the scenario allows us to determine what Eve, the eavesdropper sees when receiving the signal from Alice. We ran the experiment outdoors in as an open space as possible, to try and minimize signal reflection. It can be seen however, that in the experiment pictures there are buildings in the vicinity when running the experiment.

The results of the experimentation

### Conclusion
(Samson)
iJam with Channel Randomization successfully achieves to protect key bits from multi-antenna eavesdroppers by creating an artificially fast-fading channel effect. This work demonstrates an improved approach to the existing iJam method who utilizes a jamming method to randomly jam one of two duplicated bits. However, iJam is found to be vulnerable to multi-antenna eavesdroppers who can utilize the spatial diversity to calculate the channel effect of the pilot symbols. Therefore, we propose a defense mechanism against such attacks by combining a channel randomization with a prediction-based channel equalization.

The channel randomization technique leverages a mechanically reconfigurable antenna that rotates to rapidly change the channel state information during transmission. The angle-of-departure (AoD) based channel estimation is used to cancel its effects for the intended receiver, and the pilot vulnerability exploited by an eavesdropper is now eliminated with our CSI channel estimation mechanism, which this allows Alice to predict and pre-equalize the channel effect for Bob. As a result, a secure establishment is created between the transmitter and reviver, while the eavesdropper views an unstable channel.


#### Equipment
- Alice
  - USRP node: Ettus N210
  - Antenna(s)[decimeter band]: WAT5VJB log-periodic (850-6500 MHz)
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
