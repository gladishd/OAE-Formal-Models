# OAE-Formal-Models: Code as Proof for Open Atomic Ethernet

This repository contains the formal, executable models that serve as the mathematical and philosophical foundation for the Open Atomic Ethernet (OAE) specification. For five decades, Ethernet has operated under the assumption that reliability begins at Layer 4, forcing applications to contend with the consequences of an unreliable fabric. This has led to a widespread fallacy: that faster links mean faster systems. In practice, modern distributed applications are not limited by raw link capacity but by round-trip latency, queuing behavior, and the chaotic contention that arises from a best-effort network.

**Our core thesis is that the industry must shift its focus from multiplexing raw bandwidth to multiplexing the transactional capacity of the link.** These notebooks are our "Code as Proof"—a collection of computational essays and simulations designed in Wolfram Mathematica to formally deconstruct the flaws of classical networking and provide a verifiable blueprint for the Dædælus architecture.

> We cannot build certainty atop silence. Timeout and retry are holdovers from a more forgiving era, where best-effort sufficed and correctness was the domain of upper layers. But at hyperscale, correctness must begin at the wire.

---

## The Models: A Computational Narrative

Each model in this repository is a chapter in our argument for a new kind of network: one built on symmetric reversibility, deterministic interactions, and conserved quantities.

### Deconstructing the Old Way: The Flaws of Contention

These models analyze the foundational protocols of conventional networking to prove, computationally, why a new approach is necessary.

* **The Metcalfe-Boggs Model:** An agent-based simulation of the original 1976 protocol. It visualizes the chaotic nature of statistical arbitration on a shared Ether, demonstrating how frequent packet collisions represent the "irreversible smash of Shannon information" and serve as the microscopic origin of unbounded tail latency. This model proves why any system built on this foundation cannot guarantee exactly-once semantics.
* **The Origin of Tail Latency:** A precise, agent-based simulation that plots the Round-Trip Time (RTT) distribution and channel utilization under contention. It provides a definitive, visual illustration of how the probabilistic design of CSMA/CD inevitably leads to the performance degradation that our own architecture eliminates.

### Building the New Way: The Dædælus Architecture

These models introduce and formally specify the core components of the Dædælus Transaction Fabric.

* **The Dædælus Efficiency Model:** This computational essay provides the definitive proof of our architecture. It contrasts traditional bandwidth-multiplexing with the **Transaction-Multiplexing** enabled by our reliable **N2N Lattice**. Using simulations of the **Reversible Snake** protocol, it demonstrates the elimination of contention and immunity to packet loss, providing the formal justification for a fabric capable of **Truncated Tail Latency**.
* **Foundations of Reversibility:** An exploration of the Spekkens Toy Model, a framework from Quantum Information Theory. This notebook serves as "Code as Proof" for the principles of **Token Dynamics** and **Reversible Subtransactions**. It provides the mathematical intuition for the epistricted registers that allow our protocols to escape the irreversible failures of conventional networking.
* **The Graph Virtual Machine & Causal Ordering:** An implementation of a **Graph Virtual Machine (GVM)** that models Leslie Lamport’s classical "happens-before" relation. This formal model of definite causal order perfectly embodies the **Forward-In-Time-Only (FITO)** thinking of traditional systems. Its inability to resolve paradox highlights the necessity of the Reversible Subtransactions central to the Dædælus philosophy.
* **FabricCalculus & Geodesic Routing:** An executable specification for a foundational component of our Transaction Fabric. We define a multi-dimensional **FabricMetricTensor** that calculates a true **TransactionalDistance** based on a weighted policy of latency, bandwidth, and link integrity. The **GeodesicTransactionRouter** then computes the optimal path across the N2N Lattice, demonstrating a resilient and policy-driven fabric.

---

## Engagement

We invite collaboration and review. These models are not static documents; they are live computational essays intended to spark discussion and drive the OAE specification forward. Please engage with them, question their assumptions, and help us architect the future.
https://www.wolframcloud.com/obj/gladishdean/Published/NBforFMS.nb
https://www.wolframcloud.com/obj/gladishdean/Published/sliceProtocolForFMS.nb
https://www.wolframcloud.com/obj/gladishdean/Published/wolfram%20cloud%20for%20sahas.nb
https://www.wolframcloud.com/obj/gladishdean/Published/wolfram%20cloud%20for%20sahas2.nb
https://www.wolframcloud.com/obj/gladishdean/Published/wolfram%20cloud%20for%20sahas3.nb
https://www.wolframcloud.com/obj/gladishdean/Published/wolfram%20cloud%20for%20sahas4.nb
https://www.wolframcloud.com/obj/gladishdean/Published/python%20ddl.nb
https://www.wolframcloud.com/obj/gladishdean/Published/python%20ddl%202.nb
https://www.wolframcloud.com/obj/gladishdean/Published/cellular%20automata%20-%20from%20classical%20computation%20to%20quantum%20error%20correction.nb
https://www.wolframcloud.com/obj/gladishdean/Published/2.%20cellular%20automata%20-%20from%20classical%20computation%20to%20quantum%20error%20correction.nb
https://www.wolframcloud.com/obj/gladishdean/Published/3.%20cellular%20automata%20-%20from%20classical%20computation%20to%20quantum%20error%20correction.nb
https://www.wolframcloud.com/obj/gladishdean/Published/4.%20cellular%20automata%20-%20from%20classical%20computation%20to%20quantum%20error%20correction.nb
https://www.wolframcloud.com/obj/gladishdean/Published/5.%20cellular%20automata%20-%20from%20classical%20computation%20to%20quantum%20error%20correction.nb
https://www.wolframcloud.com/obj/gladishdean/Published/6.%20OAE-SPEC-MAIN.nb
https://www.wolframcloud.com/obj/gladishdean/Published/7.%20java.nb
https://www.wolframcloud.com/obj/gladishdean/Published/8.%20sahas.nb
https://www.wolframcloud.com/obj/gladishdean/Published/10Ants.nb
https://www.wolframcloud.com/obj/gladishdean/Published/6.%200AE-SPEC-MAIN.nb
