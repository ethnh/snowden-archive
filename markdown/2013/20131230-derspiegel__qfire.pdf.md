# Getting Close to the 

## A. Forward-based Defense with QFIRE June 3, 2011

## QFIRE Pilot Lead NSA/Technology Directorate

Derived From: NSA/CSSM 1-52
Dated: 20070108
Declassify On: 20360401
# Abstract 

${ }^{70}$ (TS//SI//REL) The goal of forward-based defense is to detect and mitigate malicious threats in real-time, as close to the source as possible. It is part of a layered defense strategy with four concentric zones: endpoint-, perimeter-, aggregation-, and forwardbased defenses. The QUANTUMTHEORY mission leverages NSA's vast system of distributed passive sensors to detect target traffic and tip a centralized command/control node. This node assesses the tip and injects a response towards the target using active TAO assets.
${ }^{72}$ (TS//SI//REL) Extremely powerful CNE/CND/CNA network effects are enabled by integrating our passive and active systems:
${ }^{70}$ resetting connections
${ }^{7}$ redirecting targets for exploitation
${ }^{7}$ taking control of IRC bots
${ }^{7}$ corrupting file uploads/downloads
${ }^{7}$ More!
${ }^{70}$ (TS//SI//REL) The success rate of these effects is largely determined by the latency from tip-to-target. QFIRE is a consolidated QUANTUMTHEORY platform under development that reduces latencies by co-locating (1) existing passive sensors with (2) local decision resolution, and (3) the ability to locally inject traffic to achieve the desired network effect.
# Topics 

$\Rightarrow$ Layered Defense Model
$\Rightarrow$ NSA TURBULENCE Architecture
$\Rightarrow$ TURMOIL passive SIGINT sensors
$\Rightarrow$ TURBINE active SIGINT command/control
$\Rightarrow$ QUANTUMTHEORY
$\Rightarrow$ Integrating passive/active systems for CNE/CND/CNA
$\Rightarrow$ QFIRE
$\Rightarrow$ Consolidated low-latency QUANTUMTHEORY capability under development for forward-based defense
Forward-based Defense NSA TURBULENCE Architecti
![img-0.jpeg](img-0.jpeg)
# Distributed Sensors: Passive 

## Callactin Accesses

TURMOIL TUTELAGE

## LIINTOTE (S//SII/REL) High-speed passive collection

systems intercept foreign target satellite, microwave, and cable communications as they transit the globe.
![img-1.jpeg](img-1.jpeg)
# TURBINE: Active Mission Management 

Accesses
TURMOIL
TUTELAGE
Implants (TAO)
(TSI/SII/REL) TURBINE provides centralized automated command/control of a large network of active implants
![img-2.jpeg](img-2.jpeg)
# QUANTUMTHEORY 

$\Rightarrow$ (TS//SI//REL) Extremely powerful CNE/CND/CNA network
![img-3.jpeg](img-3.jpeg)
effects are enabled by integrating our passive and active systems:
$\Rightarrow$ Resetting connections (QUANTUMSKY)
$\Rightarrow$ Redirecting targets for exploitation (QUANTUMINSERT)
$\Rightarrow$ Taking control of IRC bots (QUANTUMBOT)
$\Rightarrow$ Corrupting file uploads/downloads (QUANTUMCOPPER)
$\Rightarrow$ (TS//SI//REL) QUANTUMTHEORY dynamically injects packets into a target's network session to achieve CNE/CND/CNA network effects.
$\Rightarrow$ Detect: TURMOIL passive sensors detect target traffic \& tip TURBINE command/control.
$\Rightarrow$ Decide: TURBINE mission logic constructs response \& forwards to TAO node.
$\Rightarrow$ Inject: TAO node injects response onto Internet towards target.
$\Rightarrow$ (TS//SI//REL) The propagation delay from tip-to-target determines the success rate of the network effect. Less Latency = More Success!
# QFIRE: Consolidate for 

## Low-Latency

$\Rightarrow$ QUANTUMTHEORY Path: site $\circ$ NSAW-TURBINE $\circ$ target
$\Rightarrow$ (TS//SI//REL) QFIRE collocates at site: sensor, decision logic, and local/regional injection capability to achieve low latency.
$\Rightarrow$ Use existing SIGINT sensors for alerting
$\Rightarrow$ Local decision resolution (local TURBINE)
$\Rightarrow$ Local/regional injection capability
$\Rightarrow$ QFIRE Path: site $\circ$ target
$\Rightarrow$ (TS//SI//REL) A low latency capability substantially increases the variety of achievable CNE/CND/CNA network effects and improves their overall effectiveness.
# QFIRE/Forward-Based Defense: 

## ![img-4.jpeg](img-4.jpeg)

Conduct time trials \& evaluate operational effectiveness
$\Rightarrow$ Develop/deploy QFIRE for high-speed SSO cable site(s)
$\Rightarrow$ Dependencies
$\Rightarrow$ Grow regional shooter infrastructure (more Points-of-Presence)
$\Rightarrow$ Develop local/regional insertion capability at SSO cable accesses
$\Rightarrow$ Enhance cloud analytics and QUANTUM missions
$\Rightarrow$ Botnet mitigation pilot effort
# QFIRE Components (1) 

## SCS

![img-5.jpeg](img-5.jpeg)
# QFIRE (1) SCS: Physical/Virtual Network Architecture 

![img-6.jpeg](img-6.jpeg)
![img-7.jpeg](img-7.jpeg)
# HTTP Web Client/Server 

- Client initiates request, then server replies
- TCP socket:
- Client: TCP SYN
- Server: TCP SYN/ACK
- HTTP 1.1 Persistent C0nnection
- Client: HTTP GET1
- Server: HTTP Response1
- Client: HTTP GET2
- Server: HTTP Response2
# QUANTUM INSERT: racing theserver 

$\Rightarrow$ Wait for client to initiate new connection
$\Rightarrow$ Observe server-to-client TCP SYN/ACK
$\Rightarrow$ Shoot! (HTTP Payload)
$\Rightarrow$ Hope to beat server-to-client HTTP Response
$\Rightarrow$ The Challenge:
$\Rightarrow$ Can only win the race on some links/targets
$\Rightarrow$ For many links/targets: too slow to win the race!
# QUANTUM INSERT: racing 

![img-8.jpeg](img-8.jpeg)

QI
# QUANTUMTHEORY 

| Latency* |  |  |
| :--: | :--: | :--: |
| Node | QUANTUMTHEOR |  |
| SAS | Ste Access System Front end \& Layer 0/1 | ? |
| Stageo | TUMULT: Demux \& Layer 2 | ? |
| Sensor | TURMOIL: Layer 3+Passive Sensor/Event Detection | 10 |
| nix | ISLANDTRANSPORT: Enterprise Message Service | 120 |
| C\&C | TURBINE: Command/Control Decision Logic | 20 |
| Diode | SJRPLUSHANGAR: High-to-Low Diode | 20 |
| CovNet | TAO Covert Network (MIDDLEMAN) | 70 |
| Inject | TAO injection implant | 75 |
| Target | Destination for CNE/CND/CNA network effect | $-$ |
| *Timing Measurements, QUANTUMTHEORY Workshop, October 2010 |  |  |
