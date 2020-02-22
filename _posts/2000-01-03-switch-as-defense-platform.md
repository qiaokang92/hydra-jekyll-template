---
title: The switch as a defense platform
author_staff_member: gerald
---


Our first step is to transform a programmable switch into a defense platform that runs a wide range of "defense apps". The key challenge lies in the limited programming model and resources in a network switch. Our key solution is to leverage software/hardware codesign, which divides a defense app into a hardware component that needs to be invoked per packet, a software component that only needs to be involved per batch, and an interface that permits bi-directional communications.

NetWarden [USENIX Security 2020] outlines design principles for software/hardware codesign for network security applications. It applies these design principles to a concrete use case: mitigating network covert channels.

Poise [USENIX Security 2020] is an advanced access control system for "context-aware" security. Poise comes with a high-level policy language, with which users can easily specify a wide range of context-aware policies. Our compiler then generates switch programs that implement these policies entirely in hardware.

Poseidon [NDSS 2020] is a programmable defense system against volumetric DDoS attacks. It has a resource management mechanism that generates optimized mappings from defenses to the defense resources---both programmable switches and server-based defense software.

NetHCF [ICNP 2019] is a defense system that detects and filters spoofed traffic at programmable switches. It relies on the mapping from source addresses and the TTL values (i.e., hopcount-based filtering) to recognize potential spoofing.
