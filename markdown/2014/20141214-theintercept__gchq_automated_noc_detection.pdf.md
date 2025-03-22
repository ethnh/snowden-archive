# TOP SECRET STRAP 2 

![img-0.jpeg](img-0.jpeg)
# TOP SECRET STRAP 2 Challenge 

- SDC 2009 - Challenged the Network Analysis community to automate the detection of Network Operations Centres
# TOP SECRET STRAP 2 

## Phase 1: Intelligent Router Configuration File Parsing

- Routers have numerous services running on them that help identify the NOC IP ranges:
- SSH
- TELNET/VTY
- SNMP
- SYSLOG
- DNS
- TACACS
- RADIUS
- Access to these services tends to be locked down by the use of Access Control Lists (ACLs)
- Configuration files provide details of how services are configured.
# TOP SECRET STRAP 2 NOCTURNAL SURGE 

- GCHQ response to challenge.
- Early Prototype that looks at only:
- ACLs for SSH/TELNET
- ACLs for VTY
![img-1.jpeg](img-1.jpeg)

# Recent Updates: 

20110118 - v0.2

- Added Server Information from TIDAL SURGE Westens Used Data for Projects and Global DB
- Added collapsible sections for above where number of Servera $>5$
- Changed colour scheme to bi-light unrecognized ACL bitmaika that do not convert to CIDR in . . . and CIDR blocks in TELLOW
![img-2.jpeg](img-2.jpeg)
![img-3.jpeg](img-3.jpeg)
![img-4.jpeg](img-4.jpeg)
# TOP SECRET STRAP 2 

GCHQ / CSEC NAC Joint tradecraft development

- During March 2011 GCHQ Analysts visited CSEC to look at the using PENTAHO for tradecraft modelling working with CSEC NAC and CSEC/H3 software developers to see if could model NOCTURNAL SURGE in PENTAHO and then implement in OLYMPIA.
- Only possible to attempt because:
- GCHQ NAC use PENTAHO
- CSEC NAC/H3 use PENTAHO
- CSEC NAC have implemented GCHQ NAC TIDAL SURGE Database Schema (DSD also have this...)
- GCHQ approach based on AS
- CSEC approach based on Country
# TOP SECRET STRAP 2 Pentaho - NOC Auto Detection 

![img-5.jpeg](img-5.jpeg)
# TOP SECRET STRAP 2 

## Phase 2: Intelligent use of Metadata

- We do not always get full configuration files to parse.
- Services between routers and NOCs run on IP/TCP/UDP
- We do create 5-TUPLE metadata from our collection
- GCHQ have prototype database - 5-Alive
- CSEC have database - HYPERION
# TOP SECRET STRAP 2 

## SNMP Protocol

![img-6.jpeg](img-6.jpeg)
# TOP SECRET STRAP 2 SNMP Protocol in 5-Alive 

## Diarised Events Activity Graphs

Options
![img-7.jpeg](img-7.jpeg)
# TOP SECRET STRAP 2 

## Further drill down on activity for identified IP

![img-8.jpeg](img-8.jpeg)
# TOP SECRET STRAP 2 

## Phase 3: Intelligent use of TELNET traffic

- Again we do not always get full configuration files. Phase 1 is based on full (or as near to full) configuration files
- GCHQ NAC collect TELNET Sessions into TERMINAL SURGE
- Collection based on TCP Port 23 (TELNET)
- Other protocols use TCP Port 23 (YMSG)
- Interaction with Routers over TCP Port 23 maybe nefarious:
- Scanning
- Password guessing
- Need to separate legitimate use from nefarious activity
- Look for signs of legitimate use.
- Successful login
- Follow on commands
# TOP SECRET STRAP 2 

From TCP Port 23 (Echo)
![img-9.jpeg](img-9.jpeg)
# TOP SECRET STRAP 2 

## To TCP Port 23

![img-10.jpeg](img-10.jpeg)
# TOP SECRET STRAP 2 

## Intelligent analysis of TELNET traffic

- The fact that login was successful for both examples means the following:
- From TCP Port 23
- To IP address is Network Management Terminal (in the NOC ?)
- To TCP Port 23
![img-11.jpeg](img-11.jpeg)
- From IP address is Network Management Terminal (in the NOC ?)
# TOP SECRET STRAP 2 

## Phase 4: Bulk Port Scanning

- We know the key services/servers running in the NOC
- Utilise HACIENDA, GCHQ's bulk port scanning capability to identify what IPs have these service ports open - additional logic to build up confidence required.
# TOP SECRET STRAP 2 

## Fusion of sources

- Aim is to bring all sources that help identify NOC IP ranges together with associated confidence.
- Different techniques provide different results due to the nature of passive access (international v's in-country for instance)
- Different techniques have different levels of reliability - therefore looking to develop aggregation with overlay of smart intelligence.
- Solution can work on not just ISP NOCs but also Mobile OMCs.
# TOP SECRET STRAP 2 

And then....enabling CNE on NOCs

- We now have IP ranges - need selectors of NOC Staff to enable QUANTUM INSERT attack against them.
- Use of GCHQ TDI capability to identify selectors coming out of IP ranges and/or identification of proxy/NAT within NOC range.
# TOP SECRET STRAP 2 

## NOC IP range search in MUTANT BROTH

## MUTANT BROTH

![img-12.jpeg](img-12.jpeg)
# TOP SECRET STRAP 2 

## NOC IP range - Target identifiers for QUANTUM INSERT

| Source IP | User-Age | Date | Time | Non <br> Routine <br> Source | Source <br> IP:HHP | Source IP Geo | Identifier <br> Type | Identifier <br> Value | Event Count (\%) |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
|  | Maolla/5.0 (X |  |  |  | 80.84:19.9:423b:d41 | 50.83:4.33:BRUSSELS:BE;TLLM | Yahoo-B-Coable |  | $(4 \%)$ |
|  | Maolla/5.0 (X | 17/05/11 | 00:02:54 |  | 80.84:19.9:423b:d41 | 50.83:4.33:BRUSSELS:BE;TLLM | Yahoo-B-Coable |  | $(2 \%)$ |
|  | Maolla/5.0 (X | 17/05/11 | 00:02:59 |  | 80.84:19.9:423b:d41 | 50.83:4.33:BRUSSELS:BE;TLLM | Yahoo-B-Coable |  | $(0 \%)$ |
|  | Maolla/4.0 (n |  |  |  |  |  |  |  | $(1 \%)$ |
|  | Maolla/5.0 (X | 17/05/11 | 00:02:59 |  | 80.84:19.9:423b:d41 | 50.83:4.33:BRUSSELS:BE;TLHV | Yahoo-B-Coable |  | $(16 \%)$ |
|  | Maolla/5.0 (Y) |  |  |  |  |  |  |  | $(4 \%)$ |
|  | Maolla/5.0 (X | 17/05/11 | 00:05:37 |  | 80.84:19.9:5eec974d | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  | $(14 \%)$ |
|  | Maolla/5.0 |  |  |  |  |  |  |  | $(0 \%)$ |
|  | Maolla/5.0 (X | 17/05/11 | 00:16:18 |  | 80.84:19.9:749134a5 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  | $(20 \%)$ |
|  | Maolla/5.0 (X |  |  |  |  |  |  |  | $(18 \%)$ |
|  | Maolla/5.0 (Y) | 17/05/11 | 00:17:58 |  | 80.84:19.9:77387b02 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  | $(3 \%)$ |
|  |  | 17/05/11 | 00:23:35 |  | 80.84:19.9:e4a90e3f | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  |  |
|  |  | 17/05/11 | 00:28:05 |  | 80.84:19.9:749134a5 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  |  |
|  |  | 17/05/11 | 00:37:34 |  | 80.84:19.9:636815d3 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  |  |
|  |  | 17/05/11 | 00:39:55 |  | 80.84:19.9:636815d3 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  |  |
|  |  | 17/05/11 | 00:47:56 |  | 80.84:19.9:477c4721 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- <br> Coakie |  |  |
|  |  | 17/05/11 | 00:54:38 |  | 80.84:19.9:423b:d41 | 50.83:4.33:BRUSSELS:BE;TLHV | Google-PREFID- |  |  |

![img-13.jpeg](img-13.jpeg)

This information is exempt from disclosure and
legislation. Refer disclosure requests to GCHC.
# TOP SECRET STRAP 2 

## Real-time picture of QI

![img-14.jpeg](img-14.jpeg)
# TOP SECRET STRAP 2 

## Questions?

![img-15.jpeg](img-15.jpeg)
