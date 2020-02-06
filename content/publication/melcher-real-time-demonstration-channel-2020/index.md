---
draft: true
title: "Real-Time Demonstration of Channel Randomization Based Orthogonal Blinding"
date: 2020-04-01
publishDate: 2019-12-09T22:03:49.470685Z
authors: ["Jordan Melcher", "Thomas Yang", "Yao Zheng", "Yanjun Pan", "Ming LI"]
publication_types: ["1"]
abstract: ""
featured: false
publication: "*IEEE INFOCOM 2020 - IEEE Conference on Computer Communications Workshops (INFOCOM WKSHPS)*"
tags: ["preprint"]
resources:
- src: 'images/scenario_01.png'
  name: scenario_01
- src: 'images/scenario_02.png'
  name: scenario_02
- src: 'images/scenario_03.png'
  name: scenario_03
- src: 'images/scenario_04.png'
  name: scenario_04
- src: 'images/scenario_05.png'
  name: scenario_05
- src: 'images/scenario_06.png'
  name: scenario_06
- src: 'images/scenario_07.png'
  name: scenario_07
- src: 'images/scenario_08.png'
  name: scenario_08
- src: 'images/scenario_09.png'
  name: scenario_09
- src: 'images/scenario_10.png'
  name: scenario_10
- src: 'images/scenario_11.png'
  name: scenario_11
- src: 'images/scenario_12.png'
  name: scenario_12
---
Orthogonal blinding based schemes for wireless physical layer security aim to achieve secure communication by injecting noise into channels orthogonal to the main channel and corrupting the eavesdropper's signal reception. These methods, albeit practical, have been proven vulnerable against multi-antenna eavesdroppers who can filter the message from the noise. The venerability is rooted in the fact that the main channel state remains stasis in spite of the noise injection, which allows an eavesdropper to estimate it promptly via known symbols and filter out the noise. Our proposed scheme leverages a reconfigurable antenna for Alice to rapidly change the channel state during transmission and a compressive sensing based algorithm for her to predict and cancel the changing effects for Bob. As a result, the communication between Alice and Bob remains clear, whereas randomized channel state prevents Eve from launching the known-plaintext attack. We formally analyze the security of the scheme against both single and multi-antenna eavesdroppers and identify its unique anti-eavesdropping properties due to the artificially created fast changing channel. We conduct extensive simulations and real-world experiments to evaluate its performance. Empirical results show that our scheme can suppress Eve's attack success rate to the level of random guessing, even if she knows all the symbols transmitted through other antenna modes.

***
## Demonstrations

***

## Experiments
### Equipment
- Alice
  - USRP node: Ettus N210 @ 10.10.3.20
  - Rotator: Calypso @ 10.10.3.133
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Bob
  - USRP node: Ettus N210 @ 10.10.3.25
  - Rotator: Daedalus @ 10.10.3.146
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Eve
  - USRP node: Ettus N210 @ 10.10.3.10;10.10.3.15
  - Antenna(s): WAT5VJB log-periodic (850-6500 MHz)
- Spectrum analyzer
  - icarus (Keysight N9010B): 10.10.3.103
- Camera
  - primary: Sony Alpha 6000
  - secondary: Canon PowerShot S95

### Personel and Tasks

| Name                | Phase One                                                   | Phase Two                          |
| ---                 | ---                                                         | ---                                |
| Thomas Yang         | move Calypso to test site, move Eve node to test site       | manage cable at Alice and Bob node |
| Marionne Casipit    | move Daedalus to test site, move Eve node to test site      |                                    |
| Dylan Anthony       | move Eve's antenna to test site, move Eve node to test site | hold reflector                     |
| Yao Zheng           | move Alice node to test site, move Eve node to test site    | move Eve node, commence experiment |
| Jordan Melcher      | move Bob node to test site, move Eve node to test site      | move Eve node, commence experiment |
| Will Bracken        | measure and mark test site                                  | bookkeeping experiment progress    |
| Samson Aggelopoulos | measure and mark test site                                  | secondary camera                   |
| Matthew Troglia     | measure and mark test site                                  | primary camera                     |

### Procedure

```python
bookkeeping = open_bookkeeping()
eve_node = open_eve_node()
primary_camera = open_primary_camera()
secondary_camera = open_secdonary_camera()

primary_camera.start()

for scenario in scenarios:
  for experiment in scenario.experiments:
    # Register experiment, Re-position, Reset
    bookkeeping.check_experiment(experiment)

    if eve_node.position != scenario.eve_position:
      eve_node.position = scenario.eve_position

    if secondary_camera.rotator_to_shoot != scenario.rotator:
      secondary_camera.rotator_to_shoot = scenario.rotator

    labview = open_labview()
    labview.reset_rotator(experiment.rotator)
    labview.input_parameters(experiment.parameters)

    screencast = open_screencast()

    # Run Experiment
    screencast.start()
    labview.start()
    secondary_camera.start()
    labview.show_sync_status()
    labview.show_csi()

    # Stop Experiment
    screencast.stop()
    labview.stop()
    secondary_camera.stop()

    # Wrap up
    labview.check_data()
    labview.close()
    screencast.close()

primary_camera.stop()

secondary_camera.close()
primar_camera.close()
eve_node.close()
bookkeeping.close()

```

### Scenario 01

{{< imgproc scenario_01 Resize "800x" >}}Scenario 01{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB[^2]    | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 01a][scenario 01a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 01b][scenario 01b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 01c][scenario 01c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 01d][scenario 01d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 01e][scenario 01e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 01f][scenario 01f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 01g][scenario 01g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 01h][scenario 01h url] |

### Scenario 02

{{< imgproc scenario_02 Resize "800x" >}}Scenario 02{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 02a][scenario 02a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 02b][scenario 02b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 02c][scenario 02c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 02d][scenario 02d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 02e][scenario 02e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 02f][scenario 02f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 02g][scenario 02g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 02h][scenario 02h url] |

### Scenario 03

{{< imgproc scenario_03 Resize "800x" >}}Scenario 03{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 03a][scenario 03a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 03b][scenario 03b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 03c][scenario 03c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 03d][scenario 03d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 03e][scenario 03e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 03f][scenario 03f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 03g][scenario 03g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 03h][scenario 03h url] |

### Scenario 04

{{< imgproc scenario_04 Resize "800x" >}}Scenario 04{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 04a][scenario 04a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 04b][scenario 04b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 04c][scenario 04c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 04d][scenario 04d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 04e][scenario 04e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 04f][scenario 04f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 04g][scenario 04g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 04h][scenario 04h url] |
                                    
### Scenario 05

{{< imgproc scenario_05 Resize "800x" >}}Scenario 05{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 05a][scenario 05a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 05b][scenario 05b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 05c][scenario 05c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 05d][scenario 05d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 05e][scenario 05e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 05f][scenario 05f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 05g][scenario 05g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 05h][scenario 05h url] |
                                    
### Scenario 06

{{< imgproc scenario_06 Resize "800x" >}}Scenario 06{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 06a][scenario 06a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 06b][scenario 06b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 06c][scenario 06c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 06d][scenario 06d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 06e][scenario 06e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 06f][scenario 06f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 06g][scenario 06g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 06h][scenario 06h url] |
                                    
### Scenario 07

{{< imgproc scenario_07 Resize "800x" >}}Scenario 07{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 07a][scenario 07a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 07b][scenario 07b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 07c][scenario 07c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 07d][scenario 07d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 07e][scenario 07e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 07f][scenario 07f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 07g][scenario 07g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 07h][scenario 07h url] |
                                    
### Scenario 08

{{< imgproc scenario_08 Resize "800x" >}}Scenario 08{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 08a][scenario 08a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 08b][scenario 08b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 08c][scenario 08c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 08d][scenario 08d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 08e][scenario 08e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 08f][scenario 08f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 08g][scenario 08g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 08h][scenario 08h url] |
                                    
### Scenario 09

{{< imgproc scenario_09 Resize "800x" >}}Scenario 09{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 09a][scenario 09a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 09b][scenario 09b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 09c][scenario 09c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 09d][scenario 09d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 09e][scenario 09e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 09f][scenario 09f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 09g][scenario 09g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 09h][scenario 09h url] |
                                    
### Scenario 10

{{< imgproc scenario_10 Resize "800x" >}}Scenario 10{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 10a][scenario 10a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 10b][scenario 10b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 10c][scenario 10c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 10d][scenario 10d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 10e][scenario 10e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 10f][scenario 10f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 10g][scenario 10g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 10h][scenario 10h url] |
                                    
### Scenario 11

{{< imgproc scenario_11 Resize "800x" >}}Scenario 11{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 11a][scenario 11a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 11b][scenario 11b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 11c][scenario 11c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 11d][scenario 11d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 11e][scenario 11e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 11f][scenario 11f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 11g][scenario 11g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 11h][scenario 11h url] |
                                    
### Scenario 12

{{< imgproc scenario_12 Resize "800x" >}}Scenario 12{{< /imgproc >}}

| Alice Gain | Bob Gain | Eve Gain | Central Frequency (Hz) | I/Q Rate | Rotator  | Rotation Speed (rpm)[^1] | Time (s) | Data                             |
| ---        | ---      | ---      | ---                    | ---      | ---      | ---                      | ---      | ---                              |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Calypso  | 1                        | 75       | [Scenario 12a][scenario 12a url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Calypso  | 3                        | 25       | [Scenario 12b][scenario 12b url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Calypso  | 1                        | 75       | [Scenario 12c][scenario 12c url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Calypso  | 3                        | 25       | [Scenario 12d][scenario 12d url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k     | Daedalus | 1                        | 75       | [Scenario 12e][scenario 12e url] |
| 9dB        | 9dB      | 9dB      | 910M                   | 750k      | Daedalus | 3                        | 25       | [Scenario 12f][scenario 12f url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k     | Daedalus | 1                        | 75       | [Scenario 12g][scenario 12g url] |
| 9dB        | 9dB      | 9dB      | 1.75G                  | 750k      | Daedalus | 3                        | 25       | [Scenario 12h][scenario 12h url] |


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

[scenario 03a url]: # ()
[scenario 03b url]: # ()
[scenario 03c url]: # ()
[scenario 03d url]: # ()
[scenario 03e url]: # ()
[scenario 03f url]: # ()
[scenario 03g url]: # ()
[scenario 03h url]: # ()

[scenario 04a url]: # ()
[scenario 04b url]: # ()
[scenario 04c url]: # ()
[scenario 04d url]: # ()
[scenario 04e url]: # ()
[scenario 04f url]: # ()
[scenario 04g url]: # ()
[scenario 04h url]: # ()

[scenario 05a url]: # ()
[scenario 05b url]: # ()
[scenario 05c url]: # ()
[scenario 05d url]: # ()
[scenario 05e url]: # ()
[scenario 05f url]: # ()
[scenario 05g url]: # ()
[scenario 05h url]: # ()

[scenario 06a url]: # ()
[scenario 06b url]: # ()
[scenario 06c url]: # ()
[scenario 06d url]: # ()
[scenario 06e url]: # ()
[scenario 06f url]: # ()
[scenario 06g url]: # ()
[scenario 06h url]: # ()

[scenario 07a url]: # ()
[scenario 07b url]: # ()
[scenario 07c url]: # ()
[scenario 07d url]: # ()
[scenario 07e url]: # ()
[scenario 07f url]: # ()
[scenario 07g url]: # ()
[scenario 07h url]: # ()

[scenario 08a url]: # ()
[scenario 08b url]: # ()
[scenario 08c url]: # ()
[scenario 08d url]: # ()
[scenario 08e url]: # ()
[scenario 08f url]: # ()
[scenario 08g url]: # ()
[scenario 08h url]: # ()

[scenario 09a url]: # ()
[scenario 09b url]: # ()
[scenario 09c url]: # ()
[scenario 09d url]: # ()
[scenario 09e url]: # ()
[scenario 09f url]: # ()
[scenario 09g url]: # ()
[scenario 09h url]: # ()

[scenario 10a url]: # ()
[scenario 10b url]: # ()
[scenario 10c url]: # ()
[scenario 10d url]: # ()
[scenario 10e url]: # ()
[scenario 10f url]: # ()
[scenario 10g url]: # ()
[scenario 10h url]: # ()

[scenario 11a url]: # ()
[scenario 11b url]: # ()
[scenario 11c url]: # ()
[scenario 11d url]: # ()
[scenario 11e url]: # ()
[scenario 11f url]: # ()
[scenario 11g url]: # ()
[scenario 11h url]: # ()

[scenario 12a url]: # ()
[scenario 12b url]: # ()
[scenario 12c url]: # ()
[scenario 12d url]: # ()
[scenario 12e url]: # ()
[scenario 12f url]: # ()
[scenario 12g url]: # ()
[scenario 12h url]: # ()

[^1]: The rotating speed is based on actual measurment instead of the input
  value to the rotator interface. For instance, the actual rotating speed is 3rpm when  the input value is 10rpm.

[^2]: The gain range of the SBX daughter board used by the experiment is 0.0
  to 31.5 dB step 0.5dB. Therefore, to set the gain to 9dB in Labview, the gain step should be 18. The WAT5VJB LPA gives approxmiately 10 dBi gain in its boom direction.
