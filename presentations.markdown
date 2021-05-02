---
layout: page
title: Presentations
permalink: /presentations/
---

# Group Presentations

### 2020

#### Reverse Engineering Apple’s BLE Continuity Protocol for Tracking, OS Fingerprinting, and Behavioral Profiling
- **Abstract**: We reverse engineer several message types of Apple’s Bluetooth Low Energy (BLE) Continuity protocol, and show that they can be used for tracking, operating system fingerprinting, and behaviorally profiling users. In particular, we identify and reverse engineer seven distinct message types, most of which are sent in response to a particular user interaction with their iOS or macOS device. Through a series of rigorous tests in a radio-frequency sterile environment, we i) determine what actions are necessary to stimulate a device to transmit these messages, ii) deduce the meanings of most fields within each message type, and iii) ascertain how operating system version updates have introduced and affected each message type. Together, this information allows an adversary within BLE transmission range to determine what actions a user is making on their device, infer what operating system version they are using, and even track users despite the use of randomized BD_ADDR. Finally, we introduce, demonstrate, and publicly release the first-ever Wireshark dissector for displaying the Continuity message types we and other security researchers have reverse engineered.
- **Authors**: Jeremy Martin, Douglas Alpuche, Kristina Bodeman, Lamont Brown, Ellis Fenske, Lucas Foppe, Travis Mayberry, Erik C. Rye, Brandon Sipes, and Sam Teplov
- **Venus**: ShmooCon 2020 - Washington, DC - January, 2020
- **Link**: [Local](/files/shmoo20.pdf)

### 2019

#### Handoff All Your Privacy: A Review of Apple's Bluetooth Low Energy Continuity Protocol
- **Abstact**: In this work, we analyze Apple’s Continuity protocol and expose multiple privacy concerns that enable tracking, as well as defeat MAC address randomization
- **Authors**: Jeremy Martin, Douglas Alpuche, Kristina Bodeman, Lamont Brown, Ellis Fenske, Lucas Foppe, Travis Mayberry, Erik C. Rye, Brandon Sipes, and Sam Teplov
- **Venue**: Privacy Enhancing Technologies Symposium - Stockholm, Sweden - July, 2019
- **Link**: [Local](/files/Handoff_All_Your_Privacy.pdf)

### 2017

#### A Study of MAC Address Randomization in Mobile Devices and When it Fails
- **Abstact**: Media Access Control (MAC) address randomization is a privacy technique whereby mobile devices rotate through random hardware addresses in order to prevent observers from singling out their traffic or physical location from other nearby devices. Adoption of this technology, however, has been sporadic and varied across device manufacturers. In this paper, we present the first wide-scale study of MAC address randomization in the wild, including a detailed breakdown of different randomization techniques by operating system, manufacturer, and model of device. We then identify multiple flaws in these implementations which can be exploited to defeat randomization as performed by existing devices. First, we show that devices commonly make improper use of randomization by sending wireless frames with the true, global address when they should be using a randomized address. We move on to extend the passive identification techniques of Vanhoef et al. to effectively defeat randomization in ∼96% of Android phones. Finally, we identify a previously unknown flaw in the way wireless chipsets handle low-level control frames which applies to 100% of devices we tested. This flaw permits an active attack that can be used under certain circumstances to track any existing wireless device.
- **Authors**: Jeremy Martin, Travis Mayberry, Collin Donahue, Lucas Foppe, Lamont Brown, Chadwick Riggins, Erik C. Rye, and Dane Brown
- **Venue**: Privacy Enhancing Technologies Symposium - Minneapolis, MN - July, 2017
- **Link**: [Local](/files/petsPres.pdf)

### 2016

#### Decomposition of MAC Address Structure for Granular Device Inference
- **Abstact**:  Common among the wide variety of ubiquitous networked devices in modern use is wireless 802.11 connectivity. The MAC addresses of these devices are visible to a passive adversary, thereby presenting security and privacy threats – even when link or application-layer encryption is employed. While it is well-known that the most significant three bytes of a MAC address, the OUI, coarsely identify a device’s manufacturer, we seek to better understand the ways in which the remaining low-order bytes are allocated in practice. From a collection of more than two billion 802.11 frames observed in the wild, we extract device and model information details for over 285K devices, as leaked by various management frames and discovery protocols. From this rich dataset, we characterize overall device populations and densities, vendor address allocation policies and utilization, OUI sharing among manufacturers, discover unique models occurring in multiple OUIs, and map contiguous address blocks to specific devices. Our mapping thus permits finegrained device type and model predictions for unknown devices solely on the basis of their MAC address. We validate our inferences on both ground-truth data and a third-party dataset, where we obtain high accuracy. Our results empirically demonstrate the extant structure of the low-order MAC bytes due to manufacturer’s sequential allocation policies, and the security and privacy concerns therein.
- **Authors**: Jeremy Martin, Erik C. Rye, and Robert Beverly
- **Venue**: Proceedings of the Annual Computer Security Applications (ACSAC) Conference - Los Angeles, CA, - December, 2016
- **Link**: [Local](/files/furiousmac-acsac16-presentation.pdf)

### 2013

#### Correlating GSM and 802.11 Hardware Identifiers
- **Abstact**: The hardware identifiers of common wireless protocols can be exploited by adversaries for both tracking and physical device association. Rather than examining hardware identifiers in isolation, we observe that many modern devices are equipped with multiple wireless interfaces of different physical types, \eg GSM and 802.11, suggesting that there exists utility in \emph{cross-protocol hardware identifier correlation}. This research empirically examines the feasibility of such cross-protocol association, concentrating on correlating a GSM hardware identifier to that of the 802.11 hardware identifier on the same device. Our dataset includes 18 distinct mobile devices, with identifiers collected over time at disparate locations. We develop correlation techniques from the perspective of two adversaries: i) limited, able to observe identifiers only in time and space; and ii) a more advanced adversary with visibility into the data stream of each protocol. We first test correlation via temporal and spatial analysis using only basic signal collection, mimicking an RF collection with no decryption or data processing capability. Using a constrained optimization algorithm over temporal and spatial data to perform matching, we demonstrate increasing association accuracy over time, up to approx 80% in our experiments. Our second approach simulates the added capability to collect, decrypt, and reconstruct specific application protocol data, and parses the data of one protocol using search terms derived from the other. With the combined techniques, we achieve 100% accuracy and precision.
- **Authors**: Jeremy Martin, Danny Rhame, Robert Beverly, and John McEachen
- **Venue**: Proceedings of the Military Communications Conference (MILCOM) - San Diego, CA - November 2013
- **Link**: [Local](/files/gsm80211correlation-milcom13-presentation.pdf)
