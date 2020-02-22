---
title: The network as a defense fleet
author_staff_member: gerald
---

Our next step aims to transform a programmable network into a defense fleet, by architecting the individual defenses developed in the first step into the network paths, and synchronizing them for network-wide attack detection and mitigation. The key challenge we need to tackle is decentralization: the defenses need to synchronize their local views and decisions with each other without going through a central controller.

FastFlex [HotNets 2019] outlines the approach that we're taking to this decentralized defense design. It proposes the abstraction of a multimode data plane, which normally operates in an optimal mode, but can enter and exit defense modes at RTT timescales upon attacks.
