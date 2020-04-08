---
draft: True
title: "Blockage Detection/mmWave Beam Allignment"
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
---
***
## Summary
With mmWave communication operating at high frequencies, it suffer from high path losses which makes comunicating over distances challenging. In order to remedy this fact, beamforming is used in order to extend the range it can communicate over while reducing the spread. This calls for a greater importance in beam allignment between the sender and receiver to ensure the beam is directed to the receiver. When operating with mmWaves, determining where blockages occur is significant as mmWave is more susceptible to being obstructed by various materials compared to lower frequencies. By taking advantage of the known locations of various receivers, one can determine the potential locations of the blockage through the signals reflected by the blockage. By analyzing the potential locations of the blockage due to multiple receivers one can determine the likely location at which the blockage lies. After determining where the obstacles are located, one can decide at which angle has the best communication path and the sender and align itself to the receiver.

***

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
- Spectrum analyzer
  - icarus (Keysight N9010B): 10.10.3.103
- Camera
  - primary: Nikon D3300


### Scene 02

{{< imgproc scenario_02 Resize "600x" >}}Scenario 02{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator | Rotation Speed (rpm)[^1] | Time (s) | Reflectors | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---     | ---                      | ---      | ---        | ---                              |
| 60dB[^2]   | 30dB     | 30dB     | 2.6GHz                 | 500k     | Calypso | 1                        | 100      | Small      | [Scenario 02a][scenario 02a url] |
| 60dB       | 30dB     | 30dB     | 1.6GHz                 | 500k     | Calypso | 1                        | 100      | Small      | [Scenario 02b][scenario 02b url] |
| 60dB       | 30dB     | 30dB     | 900MHz                 | 500k     | Calypso | 1                        | 100      | Small      | [Scenario 02c][scenario 02c url] |
| 60dB       | 30dB     | 30dB     | 2.6GHz                 | 500k     | Calypso | 1                        | 100      | Large      | [Scenario 02d][scenario 02a url] |
| 60dB       | 30dB     | 30dB     | 1.6GHz                 | 500k     | Calypso | 1                        | 100      | Large      | [Scenario 02e][scenario 02b url] |
| 60dB       | 30dB     | 30dB     | 900MHz                 | 500k     | Calypso | 1                        | 100      | Large      | [Scenario 02f][scenario 02c url] |



***
## Demonstrations

[data url]: # (week urls)

[scenario 02a url]: # ()
[scenario 02b url]: # ()
[scenario 02c url]: # ()
[scenario 02d url]: # ()
[scenario 02e url]: # ()
[scenario 02f url]: # ()


[^1]: The rotating speed is based on actual measurement instead of the input
  value to the rotator interface. For instance, the actual rotating speed is 3rpm when  the input value is 10rpm.

[^2]: The gain range of the SBX daughter board used by the experiment is 0.0
  to 31.5 dB step 0.5dB. Therefore, to set the gain to 9dB in Labview, the gain step should be 18. The WAT5VJB LPA gives approximately 10 dBi gain in its boom direction.
