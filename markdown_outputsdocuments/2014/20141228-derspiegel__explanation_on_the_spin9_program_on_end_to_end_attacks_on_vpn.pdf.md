# Fielded Capability: End-to-End VPN SPIN 9 Design Review 

![img-0.jpeg](img-0.jpeg)

The overall classification for this brief is:
TOPSECRET//COMINT//REL USA, AUS, CAN, GBR, NZL//20320108
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Current Fielded Capability

- (TS//SI//REL) All current TURMOIL Virtual Private Network (VPN) capabilities are fielded as Spin 6 Red Architecture software running on Red Architecture hardware.

VPN Metadata

## Red

TEC No capability after Blue transition on 17-Sep

YRS
SSO
MHS Live
MHS Dev

No capability

## VPN Decryption

## Red

No capability after Blue transition on 17-Sep

No capability
No capability
Red
No capability
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Spin 9 Objectives

- (S//SI//REL) The Spin 9 Objective for the TURBULENCE (TU) VPN Private capability is to transition to the Blue Architecture.
- (S//SI//REL) Spin 9 VPN will implement a redesign of the decryption flow that reallocates some functionality between TURMOIL, the VPN Attack Orchestrator (VAO), and the VPN Metrics service.
- (U) Deliver all capabilities as deployable at the end of Spin 9.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Capabilities

- (TS//SI//REL) The TU VPN capability will implement an operational capability to detect and decrypt selected communications that are encrypted using IP security (IPsec) algorithms and protocols. It will forward the unencrypted content to followon processing systems.
- (TS//SI//REL) The TU VPN capability will collect metadata about IPsec Internet Key Exchange (IKE) events and forward the metadata to follow-on SIGINT Development (SIGDEV) systems.
# VPN Spin 9 Fielded Capability Upgrade 

## (U//FOUO) Exploited Protocols

(TS//SI//REL) IPsec automatic key management protocols establish security associations between communicants. A security association (SA) is a relationship between a source and a destination that includes a session key and other parameters. The VPN capability exploits the following key management protocols:

- (U) ISAKMP - Internet Security Association and Key Management Protocol (RFC2407, RFC2408) provides the authentication and key exchange framework.
- (U) IKE - Internet Key Exchange (RFC2409) provides the authentication and key exchange mechanisms.
# VPN Spin 9 Fielded Capability Upgrade 

## (U//FOUO) Exploited Protocols (continued)

(TS//SI//REL) IPsec security protocols provide integrity, confidentiality, and authentication for higher layer IP protocols. IPsec security protocols use security associations previously established either manually or by automatic key management protocols (IKE). The VPN capability targets SA's that are established by IKE. The VPN capability exploits the following security protocol:

- (U) ESP - Encapsulating Security Payload (RFC2406) provides traffic confidentiality (via encryption) and optionally provides authentication and integrity protection.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) IPsec Operation (Alice $\Rightarrow$ Bob)

![img-1.jpeg](img-1.jpeg)

- (U) An SA is identified by a 4-tuple <SrclP, DstIP, SPI, SecurityProtocol>, where the SPI (Security Parameter Index) is chosen by DstIP for SA uniqueness.
- (U) The Bi-directional ISAKMP SA is negotiated in Phase1 and protects the ESP key negotiations in Phase2.
- (U) A Uni-directional ESP SA is negotiated in Phase2 and is used to protect the user's cleartext.
- (U) Reverse communication (Bob $\Rightarrow$ Alice) requires a separate ESP SA and is negotiated using the same ISAKMP SA as used for (Alice $\Rightarrow$ Bob).
# VPN Spin 9 Fielded Capability Upgrade 

## (U) IPsec Modes

![img-2.jpeg](img-2.jpeg)

## (U) Transport Mode

- (U) Original IP Header is preserved
- (U) ESP Header and Trailer encapsulate and encrypt remaining IP Packet
![img-3.jpeg](img-3.jpeg)
(U) Tunnel Mode
- (U) Security Gateway at source encapsulates, encrypts, and adds new IP Header to original packet.
- (U) Security Gateway at destination recovers and forwards original packet.
- (U) Identities of traffic source and destination is concealed
- (U) Extra padding also may be added to hide packet size
# VPN Spin 9 Fielded Capability Upgrade 

## (S//SI//REL) TU VPN Products

X (TS//SI//REL) Bundled decrypt are the decrypted packets from an ESP Security Association prior to any session or application processing.

- (TS//SI//REL) Sessionized decrypted packets are the decrypted packets that have been recursively processed by the TURMOIL Stage 1 sessionizer for SIGDEV.
- (S//SI//REL) Selected application sessions are the recursed TURMOIL sessions that have been selected by KEYCARD strong selection and subsequently processed by TURMOIL Stage 2 application processing.
- (S//SI//REL) IPsec metadata are derived from IKE events for VPN SIGDEV.
- (S//SI//REL) VPN metrics are produced by CES CA components for internal use.
# VPN Spin 9 Fielded Capability Upgrade 

## (S//SI//REL) TU VPN Product Dataflows

X(TSI/SI//REL) Bundled decrypt are delivered directly to WEALTHYCLUSTER 2.0 (WC2.0) via TUBE from TURMOIL as packets for application processing that is not available in TURMOIL.

- (TSI/SI//REL) Sessionized decrypted packets are delivered without selection (full-take) to XKEYSCORE from TURMOIL for target SIGDEV.
- (S//SI//REL) Selected application sessions are delivered to PRESSUREWAVE via TUBE format conversion and EXOPUMP where data and metadata object are created and inserted into PWV for legacy analytics and analysis tools.
- (S//SI//REL) IPsec metadata are delivered to TOYGRIPPE via PWV where an analytic converts IPsec metadata to TGIF format and pushes it to TOYGRIPPE.
- (S//SI//REL) VPN metrics are delivered to CA Resources by the TURMOIL PIQ blade via CES firewall.
# VPN Spin 9 Fielded Capability Upgrade 

## (S//SI//REL) TU VPN Product Retrieval Mechanisms

## (S//SI//REL) WC2.0

- An analyst uses the AGILITY interface on WC2.0 to view selected traffic as the intended recipient would see it.


## - (S//SI//REL) PRESSUREWAVE

- The PRESSUREWAVE analytic and standing query pulls, reformats, and pushes metadata objects to TOYGRIPPE.


## - (S//SI//REL) TOYGRIPPE

- A SIGDEV analyst uses the TOYGRIPPE query interface to pull VPN metadata.
# VPN Spin 9 Fielded Capability Upgrade 

## (U//FOUO) Selection Mechanisms

- (S//SI//REL) Protocol Selection - Identify VPN traffic in IP traffic
- IKE: version=4, 0x05shdrLen $\leq 0 x f f$, nxtProtocol=17, srcPort=500, dstPort=500
- ESP: version=4, hdrLen=5, nxtProtocol=50
- (S//SI//REL) Session Selection - Identify session packets in VPN traffic
- IKE: srcIP, dstIP, srcPort, desPort, nxtProtocol (5-tuple)
- ESP: srcIP, dstIP, SPI
- (TS//SI//REL) Target Selection - Identify, select, and task target in VPN sessions
- KEYCARD performs target selection lookup with IP selectors
- KEYCARD lookup result determines tasking disposition:
- Not TRANSFORM (no action)
- TRANSFORM (decrypt)
- TRANSFORM+SURVEY (decrypt and send to XKEYSCORE)
- TRANSFORM+FORWARD $\mathcal{X}$ dno actionl send to WC2.0)
- TRANSFORM+SURVEY+FORWARD (decrypt and send to XKEY $\$ WC2.0$ )
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Design Constraints

(TS//SI//REL) Spin 9 VPN will use the following components:

| Capability | Component | Function | Developer |
| :--: | :--: | :--: | :--: |
| VPN <br> Identification and <br> Decryption | $\times$ WC2.0 | Receive bundled decrypt for application processing | TU |
|  | VPN Attack Orchestrator (VAO) | Provides IKE / ESP matching functionality. It communicates with the PIQ-Blade and is located behind the CES Firewall. | $\begin{gathered} \text { CES/SAO/ } \\ \text { Txx } \end{gathered}$ |
| VPN <br> Metadata | TOYGRIPPE | Receives VPN SOTF Metadata via PRESSUREWAVE | CES/ESO |
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Delivery Constraints

(TS//SI//REL) Spin 9 VPN will use the following delivery mechanisms:

| Capability | Product | Format | Mechanism |
| :--: | :--: | :--: | :--: |
| VPN <br> Identification and <br> Decryption | XBundled decrypt for WC2.0 | SOTF | MAILORDER |
|  | Sessionized decrypted packets from TURMOIL Data Store to XKEYSCORE | SOTF | Socket |
| VPN <br> Metadata | VPN IKE setup metadata for PRESSUREWAVE | SOTF | Socket via TUBE and EXOPUMP |
|  | VPN IKE setup metadata for TOYGRIPPE | TGIF | MAILORDER via VPN Analytic |
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Management Constraints

- (S//SI//REL) All VPN deployments must be approved by Chief CES.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Second and Third Party Constraints

- (TS//SI//REL) Spin 9 VPN identification and decryption capability will not deploy to Third Party TU Sites.
- (U//FOUO) Spin 9 VPN metadata capability will deploy to all TU sites.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) What Spin 9 VPN will do

- (S//SI//REL) Packet Detection
- Detect IKE exchanges
- Detect ESP packets
- (S//SI//REL) IPsec Metadata Flow
- Bundle all detected IKE with SRI and send to PWV
# VPN Spin 9 Fielded Capability Upgrade 

## (U) What Spin 9 VPN will do (continued)

## - (TS//SI//REL) ESP Decryption Flow

- When IKE exchange is observed, lookup IP addresses in KEYCARD. If tasked for collection, forward to VAO.
- When ESP is observed, lookup IP addresses in KEYCARD. If tasked for collection, request key from VAO.
- If decrypt key is provided by VAO, decrypt ESP packet.
- Send VPN decrypt metrics to CES VPN Metrics Service in CA Enclave.
- Recurse decrypted packets to find identifiers tasked for TURMOL processing.
- Send selected sessions to PWV via TUBE and EXOPUMP.
- Sessionize all decrypted packets and pass to XKEYSCORE for SIGDEV.

Forward all decrypted packets to WC2.0 for additional application processing.

- Process only Tunnel mode ESP packets.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) What Spin 9 VPN will not do

- (S//SI//REL) Will not process IPsec in other protocol implementations
- Will not perform pattern-based IKE / ESP detection.
- Will not process TCP/500, UDP/4500, or TCP/4500 implementations.
- Will not process IKEv2 (RFC4306).
- (S//SI//REL) Will not process non-IPsec based VPNs
- TU VPN capability will only process IPsec based VPNs.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) End-to-end test

- (TS//SI//REL) IKE and ESP test packets must use coordinated security associations
- (S//SI//REL) Use both synthetic (lab generated) and live collect test data
- (S//SI//REL) Live test data may only be processed through PIQ blade
- (TS//SI//REL) Test data characterization must include:
- 5-tuples (sourceIP, destinationIP, protocol, sourcePort, destinationPort)
- Number of IKE packets
- Number of ESP packets
- Unencrypted ESP payload content
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Test Scenarios

-(S//SI//REL) "Sunny Day" Scenarios. Single VPN with all IKE/ESP packets available and VPN Match. Exercise KEYCARD tasking option combinations.

- (TS//SI//REL) Transform - Decrypt to PRESSUREWAVE; IKE to TOYGRIPPE
- (TS//SI//REL) Transform \& Survey - Decrypt to PRESSUREWAVE \& XKEYSCORE; IKE to TOYGRIPPE
- (TS//SI//REL) Transform \& Forward - Decrypt to PRESSUREWAVE \& XWEALTHYCLUSTER 2.0; IKE to TOYGRIPPE
- (TS//SI//REL) Transform \& Survey \& Forward - Decrypt to PRESSUREWAVE, XKEYSCORE, \& WEALTHYCLUSTER 2.0; IKE to TOYGRIPPE
- (S//SI//REL) Not Transform - IKE to TOYGRIPPE
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Test Scenarios (continued)

- (U) Failure Scenarios.
- (TS//SI//REL) ESP Decryption fails because bad key is returned by VAO.
- (S//SI//REL) VAO responds with no key recovered.
- (S//SI//REL) VAO key response timeout.
- (S//SI//REL) VAO key response received after response timeout.
- (S//SI//REL) VAO response received after TDS hold time expires and ESP is not available.
- (S//SI//REL) Phase 1 and Phase 2 IKE is complete, but no ESP is collected.
- (S//SI//REL) ESP is collected, but no IKE is collected.
# VPN Spin 9 Fielded Capability Upgrade 

## (U) Test Scenarios (continued)

- (S//SI//REL) Miscellaneous Scenarios.
- (S//SI//REL) Multiple, rapid (< 30 second) Phase 2 re-keys for same initiator / responder pair.
- (S//SI//REL) Two VPN sessions collected concurrently for same IP source.
- (TS//SI//REL) Decryption flow can be disabled.
- (S//SI//REL) IKE Metadata flow can be disabled.
# VPN Spin 9 Development \& Integration Activities 

![img-4.jpeg](img-4.jpeg)
![img-5.jpeg](img-5.jpeg)
# VPN SPIN 9 Metadata Dataflows 

![img-6.jpeg](img-6.jpeg)
![img-7.jpeg](img-7.jpeg)
TOP SECRET//COMINT//20320108
![img-8.jpeg](img-8.jpeg)
# VPN Spin 9 Metadata Design Details 

![img-9.jpeg](img-9.jpeg)
# VPN Spin 9 Decryption Design Details 

![img-10.jpeg](img-10.jpeg)
# VPN Spin 9 Interfaces 

| I/ | Source | Destination | Content | Format | Schema / ICD | Changes | Transport |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| VPN1 | TURMOIL | KEYCARD | Selector Query/Response | Binary | cns.xsd | No | Socket |
| VPN2 | PIQ Blade | CES | VPN Metrics | SOAP/HTTPS | VPNMetrics.xsd | Yes | Socket (SSL) |
| VPN3 | PIQ Blade | CES VAO | ESP Crypto-variable Request/Response | SOAP/HTTPS | VAOESP.xsd | Yes | Socket (SSL) |
| VPN4 | PIQ Blade | CES VAO | IKE Message | SOAP/HTTPS | VAOIKE.xsd | Yes | Socket (SSL) |
| VPN5 | TML Home | TUBE | IKE Data/Metadata | SOTF | DataBundleOutput.xsd VPNDataBundle.xsd | Yes | Socket |
| VPN6 | TML Home | TUBE | Selected Session, Decrypted \& Recursively Processed | SOTF | TURMOIL/core VPNDecrypt.xsd | Yes | Socket |
| VPN7 | TML Home | XKEYSCORE | Decrypted Session | SOTF | TURMOIL/core VPNDecrypt.xsd | Yes | Socket |
| VPN8 | TUBE | EXOPUMP | IKE Data/Metadata | SOTF | DataBundleOutput.xsd VPNDataBundle.xsd | Yes | MAILORDER |
| VPN9 | TUBE | EXOPUMP | Selected Session, Decrypted \& Recursively Processed | SOTF | TURMOIL/core VPNDecrypt.xsd | Yes | MAILORDER |
| VPN10 | EXOPUMP | PWV | IKE Data/Metadata | SOTF | DataBundleOutput.xsd VPNDataBundle.xsd PWV Schema | Yes | ITx |
| VPN11 | EXOPUMP | PWV | Selected Session, Decrypted \& Recursively Processed | SOTF | TURMOIL/core VPNDecrypt.xsd PWV Schema | Yes | ITx |
| VPN12 | PWV | VPN Analytic | IKE Data/Metadata | SOTF | DataBundleOutput.xsd VPNDataBundle.xsd PWV Schema | Yes | ITx |
| VPN13 | VPN Analytic | TOYGRIPPE | IKE Data/Metadata | TGIF | TGIF ICD | No | MAILORDER |
| VPN14 | TML Home | TEC WC2.0 | Bundled Decrypt | SOTF | TURMOIL/core VPNDecreat.xsd | Yes | MAILORDER |
# VPN Specific BME 

| Tag | ID | Type | Value | Context | Description |
| :--: | :--: | :--: | :--: | :--: | :--: |
| vpnID | 900791 | string | xxxxxxxx-xxxx-xxxx-xxxxxxxxxxx | - Recursed packets <br> - XKEYSCORE session <br> - WC2.0 decrypt | 16-byte Universally Unique ID that associates IPsec packets in processing history |
| protocolNamespace | 900667 | string | 'ipsec/ike' | - PWV Metadata | Identify IPsec as transport protocol layer |
| keyExchange | 600533 | string | 'IKE' | - PWV Metadata | Flags IPsec IKE event |
| espspi | 55002 | uint32 | xxxxxxxx | - XKEYSCORE session - WC2.0 decrypt | 4-byte SPI from ESP packet |
| nextProtocol | 37007 | uint8 | IPTUNNEL=4 | - XKEYSCORE session - WC2.0 decrypt | Identifies IP Tunnel in processing history |
| appID | 114000 | string | 'vpn/esp' | - XKEYSCORE session - WC2.0 decrypt | Identifies VPN/ESP in XKEYSCORE Session |
| ikeCookie | 900683 | string | 8 chars | - PWV Metadata | Destination cookie from IKE packet |
| ikePayload | 900682 | string | 68 chars | - PWV Metadata | Raw payload extracted from IKE packet |
| survey | 900790 | string | 'vpn/esp' | - XKEYSCORE session | Identifies VPN/ESP in protocol history as weakly selected indicating session should not be forwarded to PRESSUREWAVE. |
| protocol | 2001 | String | 'vpn/esp' | - Recursed packets <br> - XKEYSCORE session <br> - WC2.0 decrypt | Identifies VPN in processing history |
# Questions?
# Background
# KEYCARD 

## (U) Inputs

- (U) Application ID: VPN
- (U//FOUO) Raw Selectors: IP addresses of sessions carrying the IKE exchange
- (U) Context: Packet IP addresses both source and destination (properly identified) with realm derived from network universe


## (U) Processing

- (S//SI//REL) Lookup raw selectors and report hit/no-hit results.
- (S//SI//REL) Return tasking for hits.


## (U) Outputs

- (U//FOUO) Evaluated Selectors:
- Hit or No-Hit indicators
- Target match data if necessary
# TURMOIL VPN Metadata Processing 

## (U) Inputs

- (U) Raw packets


## (U) Processing

- (S//SI//REL) Detect IKE exchanges at UDP source and destination ports 500
- (S//SI//REL) Extract IP addresses, responder cookie, message ID, ISAKMP payload
- (S//SI//REL) Bundle all IKE detect messages with SRI


## (U) Outputs

- (S//SI//REL) SOTF object containing metadata and IKE packets
# TURMOIL VPN Decrypt Processing 

## (U) Inputs

- (U) Raw packets
- (U) Selection results from KEYCARD


## (U) Processing

- (S//SI//REL) Detect ESP packets and extract IP addresses and SPI
- (S//SI//REL) Match tasked IKE exchange packets with an ESP packet stream
- (S//SI//REL) Generate UUID and assign to VPNID for unique exchange ID
- (S//SI//REL) Send Crypto-variable Request to the CES VAO
- (TS//SI//REL) If the key is returned, decrypt the ESP packets
- (TS//SI//REL) Send decrypt metrics to the CES VPN Metrics service
- (TS//SI//REL) Recurse all decrypted packets from the VPN.
- (TS//SI//REL) Sessionize all decrypted packets, pass sessions to XKEYSCORE
X (TS//SI//REL) Forward all decrypted packets to a WC2.0 for application processing.


## (U) Outputs

X (TS//SI//REL) Decrypted packets to a WC2.0

- (TS//SI//REL) Decrypt metrics to VAO
- (TS//SI//REL) Sessionized decrypted packets to XKEYSCORE
- (S//SI//REL) Selected application SOTF
# XKEYSCORE 

## (U) Inputs

- (S//SI//REL) Sessionized collect in SOTF format.


## (U) Processing

- (S//SI//REL) Recovers and archives session content. Databases metadata for query by analysts. XKEYSCORE can also perform keyword scanning and optionally forward selected data back to PINWALE. Presence tips can also be sent to TRAFFICTHIEF.
# TUBE (ID and Decryption) 

## (U) Inputs

- (U) SOTF objects.


## (U) Processing

- (C//SI//REL) Defragments fragmented sessions, creating an SOTF object with the complete session.
- (C//SI//REL) Examines the BME to determine if the session should go to PWV.
- (C//SI//REL) Creates a new SOTF object, placing the received or defragged SOTF object into the data section. The BME of the newly created object contains classification metadata*, as well as certain fields such as sessionID and signalUpTime replicated from the BME of the original received SOTF object.
* NOTE: Classification metadata needs more discussion to determine appropriate origination. TURMOIL may assume some responsibilities.
- (U) Determines appropriate routing (MAILORDER FDI) and forwards the new SOTF object to EXOPUMP via MAILORDER.
- (U) Optionally (configurable) wrap multiple objects destined for EXOPUMP/PWV into one MAILORDER file to reduce the number of individual files transmitted.


## (U) Outputs

- (U) SOTF objects.
# TUBE (Metadata) 

## (U) Inputs

- (U) SOTF objects.


## (U) Processing

- (C//SI//REL) Examines the BME to determine if the session should go to PWV.
- (U) Determines appropriate routing (MAILORDER FDI) and forwards the new SOTF object to EXOPUMP via MAILORDER.
- (U) Optionally (configurable) wrap multiple objects destined for EXOPUMP/PWV into one MAILORDER file to reduce the number of individual files transmitted.


## (U) Outputs

- (U) SOTF objects.
# EXOPUMP 

## (U) Inputs

- (U) SOTF object from TUBE via MAILORDER.


## (U) Processing

- (U) Extracts metadata from SOTF records for PWV XML metadata.
- (U) Inserts SOTF objects and XML metadata into PWV.


## (U) Outputs

- (U) PRESSUREWAVE metadata object.
# PRESSUREWAVE 

## (U) Inputs

- (S//SI//REL) VPN metadata including IKE payload objects with associated metadata represented in XML.
- (U//FOUO) Selected application data objects with associated metadata represented in $x \mathrm{ml}$.


## (U) Processing

- (S//SI//REL) PWV hosts a persistent (or standing) query created by the VPN analytic. When new metadata arrives that matches the query, the VPN analytic is notified and pulls the associated metadata and IKE packets for further processing.
- (U//FOUO) PWV serves as data store for TU analytics


## (U) Outputs

- (S//SI//REL) The metadata and IKE packets are forwarded to VPN analytic via ITx (JMS messaging service).
# VPN Analytic 

## (U) Inputs

- (S//SI//REL) Persistent query to detect VPN metadata/IKE packets in PRESSUREWAVE
- (S//SI//REL) SOTF files containing IKE packets


## (U) Processing

- (U//FOUO) Convert SOTF to TGIF records


## (U) Outputs

- (S//SI//REL) MAILORDER files with TGIF records containing intercepted IKE packets
# TOYGRIPPE 

## (U) Inputs

- (U//FOUO) TGIF ("The Grand Input Format") records based on TML collected metadata.


## (U) Processing

- (U//FOUO) TOYGRIPPE 3.2 system accepts TGIF files sent by MAILORDER as bundled "tar" files.
- (TS//SI//REL) TOYGRIPPE unbundles, validates, and stores the VPN metadata from the TGIF files into a database for later access by Analysts primarily through a web browser interface. TOYGRIPPE supports data processing and storage for PPTP and IPSec VPN metadata records.
# VAO 

## (U) Inputs

- (S//SI//REL) IKE packets
- (S//SI//REL) ESP Crypto-variable (CV) Requests


## (U) Processing

- (S//SI//REL) Generates ESP SA CV's from IKE packets
- (S//SI//REL) Matches ESP SA CV requests with generated CV's
- (S//SI//REL) Responds to ESP SA CV requests
(U) Outputs*
- (S//SI//REL) ESP Crypto-variable Response
* Note: VAO requests that multiple ESP packets also be sent for each session
# VPN Metrics 

## (U) Inputs

- (S//SI//REL) PIQ Blade VPN Processing Metrics
(U) Processing
- (S//SI//REL) Internal to CES/CA Enclave
# (U) Inputs 

- (S//SI//REL) Bundled decrypted packets in SOTF format via MAILORDER.


## (U) Processing

- (U) Signal identification
- (S//SI//REL) Protocol recognition, processing and sessionization
- (C//SI//REL) Application identification and processing
- (C//SI//REL) Link characterization aggregation
- (U//FOUO) Filtering, selection, and forwarding
- (U//FOUO) Strong selection
- (S//SI//REL) Persona session association
- (S//SI//REL) Session association
- (S//SI//REL) IP Decompression
- (S//SI//REL) Contact chaining
