---
title: "BBRv3 in the Public Internet: A Boon or a Bane?"
collection: publications
category: conferences
permalink: /publication/2024-ANRW-BBRv3
excerpt: "The third version of the Bottleneck-Bandwidth and Round-trip (BBR) algorithm, BBRv3, is now the default CCA for all public Internet traffic from google.com and YouTube. This work builds upon prior research to examine BBRv3's ability to coexist with Cubic flows by taking loss, in the form of explicit congestion notification (ECN) signals, into account. Our evaluations reveal that, when ECN is enabled, a single BBRv3 flow can acquire more than ~99% of the bandwidth even when competing with five Cubic flows. These findings have crucial implications for using BBRv3 in the public Internet."
date: 2024-07-20
venue: "Proceedings of the Applied Networking Research Workshop"
citation: "Zeynali, Danesh, Weyulu, Emilia N., Fathalli, Seifeddine, Chandrasekaran, Balakrishnan, and Feldmann, Anja. (2024). 'BBRv3 in the Public Internet: A Boon or a Bane?' Proceedings of the Applied Networking Research Workshop."
paperurl: "https://dl.acm.org/doi/abs/10.1145/3673422.3674889"
---

The Bottleneck-Bandwidth and Round-trip (BBR) congestion control algorithm was introduced by Google in 2016. Unlike prior congestion-control algorithms (CCAs), BBR does not rely on signals that are weakly correlated with congestion (e.g., packet loss and transient queue delay). Instead, it characterizes a path using two parameters, bottleneck bandwidth and round-trip propagation time, and is designed to converge with a high probability to Kleinrock’s optimal operating point.

This paper focuses on characterizing the promises and potential of the third, and most recent, revision of BBR—introduced to the public in July 2023. We empirically evaluate BBRv3’s performance across a range of network scenarios, e.g., considering different buffer sizes, round-trip times, packet losses, and flow-size distributions.

In our evaluations, we find that BBRv3 enables competing flows to converge to their fair shares quicker than prior versions. If these flows, however, do not start (or arrive at the bottleneck) at the same time, we also observe that its convergence time deteriorates substantially. We note that BBRv3 (similar to BBRv2) is biased towards long-RTT flows; they receive a higher bandwidth than a competing short-RTT flow, regardless of which flow starts first. We observe that BBRv3 struggles to co-exist with loss-based CCAs such as Cubic; it offers little to no room for Cubic flows to co-exist even if flow RTTs are similar.
