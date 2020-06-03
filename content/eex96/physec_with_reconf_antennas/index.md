---
title: "Implementation of Channel Randomizing Orthogonal Blinding"
subtitle: "Spring, 2020"
date: 2020-01-10T00:00:00-10:00
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
authors: ["Will Bracken", "Marionne Casipit", "Mark Kwon", "Yao Zheng"]
tags: ["eex96", "wireless", "SDR", "current", "featured"]
resources:
- src: 'images/scenario_01.png'
  name: scenario_01
- src: 'images/scenario_02.png'
  name: scenario_02
abstract: 'This project implements ROBin: Channel Randomizing Orthogonal Blinding, an enhanced wireless physical layer security scheme robust to known-plaintext attack.'
---
## Experiments
### Equipment
- Alice
  - USRP node: Ettus N210 @ 10.10.3.10
  - Rotator: Calypso @ 10.10.3.133
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Bob
  - USRP node: Ettus N210 @ 10.10.3.25
  - Rotator: Daedalus @ 10.10.3.146
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Eve
  - USRP node: Ettus N210 @ 10.10.3.20;10.10.3.15
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Spectrum analyzer
  - icarus (Keysight N9010B): 10.10.3.103
- Camera
  - primary: Nikon D3300

### Scene 01

{{< imgproc scenario_01 Resize "600x" >}}Scenario 01{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---     | ---                      | ---      | ---                              |
| 30dB[^2]   | 0dB      | 0dB      | 2.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 01a][scenario 01a url] |
| 30dB       | 0dB      | 0dB      | 1.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 01b][scenario 01b url] |
| 30dB       | 0dB      | 0dB      | 3.6G                   | 500k     | Calypso | 3                        | 100      | [Scenario 01c][scenario 01c url] |

### Scene 02

{{< imgproc scenario_02 Resize "600x" >}}Scenario 02{{< /imgproc >}}

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
