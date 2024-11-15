---
title: "Promises and Potential of BBRv3"
collection: publications
category: conferences
permalink: /publication/2024-PAM-BBRv3
excerpt: "The Bottleneck-Bandwidth and Round-trip (BBR) congestion control algorithm was introduced by Google in 2016. Unlike prior congestion-control algorithms (CCAs), BBR does not rely on signals that are weakly correlated with congestion (e.g., packet loss and transient queue delay). Instead, it characterizes a path using two parameters, bottleneck bandwidth and round-trip propagation time, and is designed to converge with a high probability to Kleinrock’s optimal operating point.
This paper focuses on characterizing the promises and potential of the third, and most recent, revision of BBR—introduced to the public in July 2023. We empirically evaluate BBRv3’s performance across a range of network scenarios, e.g., considering different buffer sizes, round-trip times, packet losses, and flow-size distributions.
In our evaluations, we find that BBRv3 enables competing flows to converge to their fair shares quicker than prior versions. If these flows, however, do not start (or arrive at the bottleneck) at the same time, we also observe that its convergence time deteriorates substantially. We note that BBRv3 (similar to BBRv2) is biased towards long-RTT flows; they receive a higher bandwidth than a competing short-RTT flow, regardless of which flow starts first. We observe that BBRv3 struggles to co-exist with loss-based CCAs such as Cubic; it offers little to no room for Cubic flows to co-exist even if flow RTTs are similar."
date: 2024-03-11
venue: "International Conference on Passive and Active Network Measurement"
citation: 'Zeynali, Danesh and Weyulu, Emilia N. and Fathalli, Seifeddine and Chandrasekaran, Balakrishnan and Feldmann, Anja. (2024). &quot;Promises and Potential of BBRv3.&quot; <i>International Conference on Passive and Active Network Measurement </i>.'
paperurl: 'https://inet-bbrv3eval.mpi-inf.mpg.de/'
---

The Bottleneck-Bandwidth and Round-trip (BBR) congestion control algorithm was introduced by Google in 2016. Unlike prior congestion-control algorithms (CCAs), BBR does not rely on signals that are weakly correlated with congestion (e.g., packet loss and transient queue delay). Instead, it characterizes a path using two parameters, bottleneck bandwidth and round-trip propagation time, and is designed to converge with a high probability to Kleinrock’s optimal operating point.

This paper focuses on characterizing the promises and potential of the third, and most recent, revision of BBR—introduced to the public in July 2023. We empirically evaluate BBRv3’s performance across a range of network scenarios, e.g., considering different buffer sizes, round-trip times, packet losses, and flow-size distributions.

In our evaluations, we find that BBRv3 enables competing flows to converge to their fair shares quicker than prior versions. If these flows, however, do not start (or arrive at the bottleneck) at the same time, we also observe that its convergence time deteriorates substantially. We note that BBRv3 (similar to BBRv2) is biased towards long-RTT flows; they receive a higher bandwidth than a competing short-RTT flow, regardless of which flow starts first. We observe that BBRv3 struggles to co-exist with loss-based CCAs such as Cubic; it offers little to no room for Cubic flows to co-exist even if flow RTTs are similar.
