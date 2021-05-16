---
draft: false
title: "Insider-Resistant Context-Based Pairing for Multimodality Sleep Apnea Test"

subtitle: "EEx96, Spring, 2021"

summary: "This EEx96 project implements SIENNA: a context-based pairing protocol for reliable multimodality sleep apnea screening tests."

tags:
- sleep apnea
- multimodalty screening 
- friendly jamming
- fuzzy commitment
- JADE ICA
- eavesdropper
- spoofing
- active project
- active eex96 project

date: 2021-05-16T00:00:00-10:00

authors:
- Stephanie Aelmore
- Samson Aggelopoulos
- Marionne Casipit
- Willy Chang
- Brian Lu
- Alana Power
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
  caption: ""
  focal_point: "Center"
  preview_only: true
  alt_text: " "

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
- name: Video
  url: https://www.youtube.com/watch?v=TWJSP7n3JsE&t=1s
- name: Slides
  url: 
- name: Dataset
  url: 

# Markdown Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

gallery_item:
 - album: highlights
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/DSC_0239.jpg
   caption: Experimental setup with two high gain antennas and a rotating antenna.


 - album: experiment
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/AoD_2_4Gs03a.png
   caption: Ground Truth vs Estimate AoD Vector Scenario 3a


 - album: results
   image: https://media.githubusercontent.com/media/gustybear-research/x96_physec_chan_ran/main/exp_2020_09_10/__images__/website/pred_2_4Gs03a.png
   caption: Measured vs Predicted CSI Magnitude Scenario 3a



---
***
# Executive Summary
(Samson) At-home screening systems for obstructive sleep apnea (OSA) utilizes contactless and contact-based sensing modalities, which allow for reliable remote chronic disease management. However, multimodality screening systems are vulnerable to wireless exploitations for device pairing as patients switch between modalities during screening tests. Malicious attacks from non-compliant patients would be able to manipulate the data by eavesdropping or spoofing the wireless signal. To mitigate all attacks, we present SIENNA, an insider-resistant context-based pairing protocol. SIENNA leverages JADE-ICA to identify a user’s respiration pattern within a multi-person environment and uses fuzzy commitment for automatic device pairing. Friendly jamming techniques would be used to prevent an insider with knowledge of respiration patterns from acquiring the pairing key. Our results show that SIENNA is able securely pair devices with more than 90% success rate under noisy environments and is robust against attackers with full knowledge context information.

***
# Presentation
{{< https://www.youtube.com/watch?v=TWJSP7n3JsE&t=1s >}}

***

# Highlights
{{< gallery-enhance album="highlights" numbered="true" caption="Project Highlights">}}

***

# Introduction
(Alana) text here

***

# Background
(Alana) text here

***

# Methodology
(Steph) text here

***

# Implementation and Experimentation
(Brian) text here

***

# Results and Analysis
(Samson) The breathing signature was quantized by utilizing Labview to generate binary fingerprints. The breathing signature is a combination of complex thorax motions, due to respiration and heartbeat movements within +/- 0.5cm to +/- 0.05cm. A quantization step size of 0.05cm at 10 sample rates per second was the best to preserve fine movements. The quality of the binary fingerprints was evaluated based on the hamming distances between fingerprints observed by different modalities. Human subjects are distinguishable based on their inhales exhales and breathing depth which can be directly translated to the hamming distances. The similarities of same subjects observed by different modalities demonstrates an average hamming distance per bit between fingerprints is around 63% within the first 6 seconds. Meanwhile, the similarities between different subject observed by different modalities results an average hamming distance per bit between fingerprints is below 5%. Overall, SIENNA can be set to around 70% to allow accurate patient tracking during modality switches. The security of the fuzzy commitment is measured by the randomness of the commitments. Our results show that the entropy per bit drops nearly by half when the key salt is converted into a commitment due to the redundancy of the human respiratory motion’s cyclic character. Other factors also include when the quantization levels increase, the granularity of the binary sequencing improves, which slightly improves the randomness of the breathing fingerprints, resulting in a higher degree of entropy in the commitments. Also, when the commitment is generated with multiple rounds of XOR operations, the entropy decreases due to the cross-correlation between fingerprint segments. SIENNA’s performance against eavesdropping and spoofing is evaluated by comparing the bit error rate (BER) at the receiver versus the aggregated BER at the attacker’s side. Our experiment showed that the jamming signal could suppress the attacker’s BER to roughly 50%, which would render an undecodable message for the attacker. 

***
# Conclusion



***
# Appendix
## Equipment
(Brian) text here

***
# Acknowledgement
This project is partially supported NSF grants CNS-1948568, W911NF-19-1-0050, IIP-1831303, IIS-1915738 and TMYTEK mmWave research initiative.




[data url]: # (data urls)

[2020_01_23_s01_1_6G_a]: https://github.com/gustybear-research/x96_physec_chan_ran/tree/main/exp_2020_01_23/s01_1_6G_a
