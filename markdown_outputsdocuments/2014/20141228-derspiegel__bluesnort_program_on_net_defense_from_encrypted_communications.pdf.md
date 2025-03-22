# (U//FOUO) Net Defense from Encrypted Communications 

E^hminm, 2012
![img-0.jpeg](img-0.jpeg)
# Increment 3 Requirement 

## SYSREQ10322.2

(S//REL) TURMOIL shall reinject decrypted IP traffic into BLUESNORT for malicious network activity detection.
# Three-Feather Solution 

GALLANTWAVE application
Same module supports NetDef and SIGINT
Supports dynamic update of targeting via UTT
Supports static target updates
GALLANTWAVE Reinjection application
Same module supports NetDef and SIGINT
Supports re-injection of decrypt into TURMOIL for detection by BLUESNORT
BLUESNORT in Stage 1 Prime application
Emits events off decrypted, re-packetized, reinjected data
# HIGH Level Data Flow 

Net Defense and SIGINT sites
![img-1.jpeg](img-1.jpeg)
# Status 

- Running on MHS DEV ESO T5 and T22
- Transform, Reinjection, Signature Hits confirmed
- Signatures need further development to produce true hits vs. false positives
- NTOC POC reviewing XKS hits to generate new signatures.
# Issues/Risks 

1. CA Servers at Net Defense Sites
" ITx Connectivity to LONGHAUL
" NTOC requires stand-up of separate dev and live ITx fabric
i. - H/W funding may be needed
ii. - Need paperwork for update to firewall - submission expected by 25 Feb
" Expected completion was 29 Feb; now delayed to TBD
" SSH connectivity
" Short term: via BLUEBOX CA Servers at Pentagon - done
" Longer term: via deployment of servers within the NTOC enclave that connect to CA Servers in the field
2. GALLANTWAVE Targeting Challenges
" MAILORDER/Ni-FI not yet available
" Mitigation: Manually load static targeting files
# CA Capabilities Planned for NCC-3 Test Events 

| Capability | DT/OA 2 (June 2012) |  | DT/OA 3 (June 2013 |  |
| :--: | :--: | :--: | :--: | :--: |
|  | Defensive <br> Sensor | SIGINT <br> Sensor | Defensive <br> Sensor | SIGINT <br> Sensor |
| CA Reinjection | No | DGO | TTENT | DGO |
# Near-term Schedule 

| Capability | Date |
| :-- | :--: |
| GW-R Gate 2 | Done (15 Feb) |
| GW-R Gate 3 | Done (29 Feb) |
| GW-R Gate 5 | 31 Mar |
| GW-R Deploy to U sites | May |
| ITx Dev Fabric at NetDef sites | 29 Feb + |
| CA Server ssh connectivity | Done via <br> Bluebox |
| Initial Live Dev Test TURTLEZOO | -May |
| GW-R Core 4.0 | May |
| GW Core 4.0 | May |
| ITx Live Fabric | TBD |
# Players 

![img-2.jpeg](img-2.jpeg)
BACKUP SLIDES
# CCA Capabilities Planned for NCC-3 Test Events 

| Capability | DT/OA 2 (June 2012) |  | DT/OA 3 (June 2013) |  |
| :-- | :--: | :--: | :--: | :--: |
|  | Defensive <br> Sensor | SIGINT <br> Sensor | Defensive <br> Sensor | SIGINT <br> Sensor |
| NETFLOW | Full Netflow | Pretty Good <br> Netflow | Full Netflow | Full Netflow |
| BLUESNORT (updates) | Yes | No | Yes | Yes |
| FULL SNORT | Yes | No (Core 4) | Yes | Yes |
| POPQUIZ | No | No | Yes | Yes |
| Performance Testing | Yes | No | Yes | Yes |
| Wireless reinjection | N/A | Yes | N/A | Yes |
| CA Reinjection | No | Yes | Yes | Yes |
| Cyber Tasking | Yes | Partial | Yes | Partial |
| Updated Cloudshield Interface | Partial | N/A | Yes | Yes |
| Metrics and Monitoring | Yes | No | Yes | Yes |

$\square$ Orange items are being revisited. Requirements without explicit TML Core 4 dependency need mission documentation to justify not being covered in DT/OA 2.
# (S//REL) Dynamic Defense Logical Diagram 

![img-3.jpeg](img-3.jpeg)
![img-4.jpeg](img-4.jpeg)
# Delivery to both XKEYSCORE and Stage 1 Prime Reinjection 

![img-5.jpeg](img-5.jpeg)
# TURMOIL <br> Stage 1 Prime Reinjection 

![img-6.jpeg](img-6.jpeg)
![img-7.jpeg](img-7.jpeg)
