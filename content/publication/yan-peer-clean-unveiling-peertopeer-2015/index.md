---
title: 'PeerClean: Unveiling Peer-to-Peer Botnets through Dynamic Group Behavior Analysis'
date: '2015-01-01'
draft: true
publishDate: '2022-08-14T03:32:14.102665Z'
authors:
- Qiben Yan
- Yao Zheng
- Tingting Jiang
- Wenjing Lou
- Y. Thomas Hou
publication_types:
- '1'
abstract: 'Advanced botnets adopt a peer-to-peer (P2P) infrastructure for more resilient command and control (C&C). Traditional detection techniques become less effective in identifying bots that communicate via a P2P structure. In this paper, we present PeerClean, a novel system that detects P2P botnets in real time using only high-level features extracted from C&C network flow traffic. PeerClean reliably distinguishes P2P bot-infected hosts from legitimate P2P hosts by jointly considering flow-level traffic statistics and network connection patterns. Instead of working on individual connections or hosts, PeerClean clusters hosts with similar flow traffic statistics into groups. It then extracts the collective and dynamic connection patterns of each group by leveraging a novel dynamic group behavior analysis. Comparing with the individual host-level connection patterns, the collective group patterns are more robust and differentiable. Multi-class classification models are then used to identify different types of bots based on the established patterns. To increase the detection probability, we further propose to train the model with average group behavior, but to explore the extreme group behavior for the detection. We evaluate PeerClean on real-world flow records from a campus network. Our evaluation shows that PeerClean is able to achieve high detection rates with few false positives.'
featured: false
publication: '*2015 IEEE Conference on Computer Communications (INFOCOM)*'
tags:
- conference
doi: 10.1109/INFOCOM.2015.7218396

links:
- name: PDF
  url: https://gustybear-websites.s3.us-west-2.amazonaws.com/publication-yan-peer-clean-unveiling-peertopeer-2015/Yan+et+al_2015_PeerClean.pdf
---

