---
title: "Green Building Innovation Cluster (GBIC) — IoT-Based Distributed MPC for Commercial HVAC"
excerpt: "Distributed MPC and IoT platform for commercial-building HVAC, deployed on an 85-zone pilot at Nanyang Technological University. Delivered 12–13% measured energy savings in occupied space.<br/><img src='/images/tbsa1.png' width='600' height='650'>"
collection: portfolio
---

Research Scientist role at NTU Singapore (2016–2018), Green Building Innovation Cluster. PI: Prof. Rong Su. [Project site](https://intelligentsystemseee.ntu.edu.sg/cpisrg/gbic/gbic_index.html).

Built and deployed an HVAC control platform in an occupied commercial building at NTU (S1-B1B office area, 85 zones, July 2018). The system implements a **Smart-Token Based Scheduling Algorithm (Smart-TBSA)** running as distributed MPC across a server plus Raspberry Pi edge fleet, and delivered **12–13% measured energy savings** relative to the legacy building automation system without replacing the underlying BAS hardware.

The technical contribution was an IoT-compliant reference architecture (hardware, software, networking, and integration with legacy BAS and a cloud back-end) plus a transformation of the centralized optimization models into a distributed active-control technique that runs on low-cost edge devices. Results published in *Applied Energy*: [An IoT Upgrade for Smart and Scalable HVAC Control in Commercial Buildings](https://www.sciencedirect.com/science/article/pii/S0306261919302582) (Png, Srinivasan, Bekiroglu, Chaoyang, Su, Poolla — 162 citations).

<br/><img src='/images/token.jpg'>

The "smartness" in Smart-TBSA comes from three additions to the optimization model: recursive online identification of per-zone thermal dynamics, predicted occupant thermal sensation, and cost/comfort trade-offs solved per-zone rather than globally. A centralized legacy BAS becomes a decentralized, adaptive control layer deployed via low-cost IoT devices without hardware replacement.

Structure of the local and central MPC:

Local MPC:
------
<br/><img src='/images/localMPC.png'>

Central MPC:
------
<br/><img src='/images/centralMPC.png'>



