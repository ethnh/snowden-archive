# UMMOIL 

## TURMOIL

## IPSEC VPN

## SESSIONIZATION

Issue No.1.

Issue Date 08/15/08

## Responsible Authority

Author
Technical P.O.C.
Product Approver.
Derived From: NSA/CSSM 1-52
Dated: 20041123
DECLASSIFY On: 20291123
Table of Contents
Revision History ..... 4
Reference Documents ..... 4
1.0 (U) SCOPE ..... 5
2.0 (S) ESP SESSIONIZATION ..... 5
2.1 (S) IP/ESP ..... 5
2.1.1 (S) Detection ..... 5
2.1.2 (S) Sessionizing. ..... 6
2.1.3 (S) The Stack ..... 6
2.2 (S) IP/AH/ESP ..... 7
2.2.1 (S) Detection. ..... 7
2.2.2 (S) Sessionizing. ..... 7
2.2.3 (S) The Stack ..... 8
3.0 (S) IKE SESSIONIZATION ..... 9
3.1 (U) IP/UDP/ ISAKMP ..... 9
3.1.1 (S) Detection. ..... 9
3.1.2 (S) Sessionizing. ..... 9
3.1.3 (S) The Stack ..... 10
3.2 (U) IP/UDP/MLLLS/ ISAKMP ..... 10
3.2.1 (S) Detection. ..... 10
3.2.2 (S) Sessionizing. ..... 11
3.2.3 (U) The Stack. ..... 12
3.3 (U) IP/TCP/ ISAKMP ..... 12
3.3.1 (S) Detection. ..... 12
3.3.2 (S) Sessionizing. ..... 13
3.3.3 (S) The Stack. ..... 14
3.4 (U) IP/TCP/MLLLS/ ISAKMP ..... 14
3.4.1 (S) Detection. ..... 14
3.4.2 (S) Sessionizing. ..... 15
3.4.3 (S) The Stack. ..... 16
4.0 (U) SUMMARY ..... 17
TOP SECRET//COMINT//REL TO USA, AUS, CAN, GBR, NZL//20291123
# REVISION HISTORY 

| Issue | Date | Author | Amendments |
| :--: | :--: | :--: | :-- |
| 0.1 | $8 / 15 / 08$ | ET | First draft of document |
|  |  |  |  |
|  |  |  |  |

## REFERENCE DOCUMENTS

1.
# 1.0 (U) SCOPE 

This document describes the sessionization requirements for the various IPSec VPN protocols processed in Turmoil. The list of IPSec protocol stacks of interest is shown here:

- IP/ESP
- IP/AH/ESP
- IP/UDP/ISAKMP
- IP/UDP/nulls/ISAKMP
- IP/TCP/ISAKMP
- IP/TCP/nulls/ISAKMP

Currently, IP/ESP, IP/UDP, and IP/TCP are successfully sessionized by the FIP. Other IPSec stacks have been observed in the field, and we have requirements to process them in Turmoil. For completeness, all of the stacks are discussed in this document, even though some are currently being processed.

## 2.0 (S) ESP SESSIONIZATION

## 2.1 (S) IP/ESP

### 2.1.1 (S) DETECTION

The AEG loads the FSPF with the following keyword and mask pair for this protocol:
keyword: 45 FF FF FF FF FF FF FF FF 32 FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF F5
mask: FF 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
# 2.1.2 (S) SESSIONIZING 

The ESP packets would be sessionized by the following set of parameters:

- IP Next Protocol $=50$ (0x32)
- IP Source Address
- IP Destination Address
- ESP SpI


### 2.1.3 (S) THE STACK

The fields utilized in sessionization are highlighted in red in the diagram below:
![img-0.jpeg](img-0.jpeg)
# 2.2 (S) IP/AH/ESP 

### 2.2.1 (S) DETECTION

The AEG loads the FSPF with the following keyword and mask pair for this protocol:

```
keyword: 45 FF FF FF FF FF FF FF FF 33 FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF
# 2.2.3 (S) THE STACK 

![img-1.jpeg](img-1.jpeg)
# 3.0 (S) IKE SESSIONIZATION 

## 3.1 (U) IP/UDP/ISAKMP

### 3.1.1 (S) DETECTION

The AEG loads the FSPF with the following keyword and mask pair for this protocol:
keyword: 45 FF FF FF FF FF FF FF FF 11 FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF
# 3.1.3 (S) THE STACK 

![img-2.jpeg](img-2.jpeg)

### 3.2 (U) IP/UDP/NULLS/ISAKMP

### 3.2.1 (S) DETECTION

The AEG loads the FSPF with the following keyword and mask pair for this protocol:
keyword: 45 FF FF FF FF FF FF FF FF 11 FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF
- IPv4 packet
- IP Header Length $=5$
- IP Next Protocol = UDP (0x11)
- 4 bytes of NULLS between the UDP and ISAKMP layers
- ISAKMP Version $=0 \times 10$
- ISAKMP Next Payload, Exchange Type, and Flags fields all have ranges of valid values
- ISAKMP Length (header + payload) < 64k

We have a similar keyword/mask pair for ISAKMP Version 9.9.

# 3.2.2 (S) SESSIONIZING 

The UDP/nulls/ISAKMP packets would be sessionized by the following set of parameters:

- IP Next Protocol = UDP (0x11)
- IP Source Address
- IP Destination Address
- UDP Source Port
- UDP Destination Port
# 3.2.3 (U) THE STACK 

![img-3.jpeg](img-3.jpeg)

### 3.3 (U) IP/TCP/ISAKMP

### 3.3.1 (S) DETECTION

The AEG loads the FSPF with the following keyword and mask pair for this protocol:
keyword: 45 FF FF FF FF FF FF FF FF 06 FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF
This indicates that the packets that satisfy the following parameters will be selected by this keyword for processing in the IKE_AEG:

- IPv4 packet
- IP Header Length $=5$
- IP Next Protocol = TCP (0x06)
- ISAKMP Version $=0 \times 10$
- ISAKMP Next Payload, Exchange Type, and Flags fields all have ranges of valid values
- ISAKMP Length (header + payload) < 64k

We have a similar keyword/mask pair for ISAKMP Version 9.9.

# 3.3.2 (S) SESSIONIZING 

The TCP/ISAKMP packets would be sessionized by the following set of parameters:

- IP Next Protocol = TCP (0x06)
- IP Source Address
- IP Destination Address
- TCP Source Port
- TCP Destination Port
# 3.3.3 (S) THE STACK 

![img-4.jpeg](img-4.jpeg)

### 3.4 (U) IP/TCP/NULLS/ISAKMP

### 3.4.1 (S) DETECTION

The AEG loads the FSPF with the following keyword and mask pair for this protocol:
keyword: 45 FF FF FF FF FF FF FF FF 06 FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF FF 100000 FF FF FF FF FF 0000
task: FF 0000000000000000 FF 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
# 3.4.3 (S) THE STACK 

![img-5.jpeg](img-5.jpeg)
# 4.0 (U) SUMMARY 

The FIP currently recognizes UDP, TCP, and ESP as valid Network Layer protocols, and currently sessionizes those packet types. The new requirement for IP/AH/ESP will require changes to the FIP to recognize AH as a valid layer, and will also require changes to the DFCE to allow those packets through.

There has been talk of having application-specific demuxes developed and inserted into the TE to perform any required sessionization beyond the Transport Layer. For example, the ESP demux would be responsible for sessionizing on Spi value.

The Table below summarizes the various protocol stacks, the parts of the stacks that are used in PPF keyword detection, and how the associated packets should be sessionized.

| Protocol Stack | Keyword Detection Layers | Sessionization Requirements |
| :--: | :--: | :--: |
| IP/ESP | IP, ESP | IP Next Protocol = 50 <br> IP Source Address <br> IP Destination Address <br> ESP Spi |
| IP/AH/ESP | IP, AH, ESP | IP Next Protocol = 51 <br> IP Source Address <br> IP Destination Address <br> AH Next Header = 50 <br> AH Spi <br> ESP Spi |
| IP/UDP/ISAKMP <br> * we have separate keywords for ISAKMP Versions 1.0 and 9.9 | IP, UDP, ISAKMP | IP Next Protocol = 17 <br> IP Source Address <br> IP Destination Address <br> UDP Source Port <br> UDP Destination Port |
| IP/UDP/suls/ISAKMP <br> * we have separate keywords for ISAKMP Versions 1.0 and 9.9 | IP, UDP, ISAKMP | IP Next Protocol = 17 <br> IP Source Address <br> IP Destination Address <br> UDP Source Port <br> UDP Destination Port |
| IP/TCP/ISAKMP <br> * we have separate keywords for ISAKMP Versions 1.0 and 9.9 | IP, TCP, ISAKMP | IP Next Protocol = 6 <br> IP Source Address <br> IP Destination Address <br> TCP Source Port <br> TCP Destination Port |
| :--: | :--: | :--: |
| IP/TCP/nulls/ISAKMP <br> * we have separate keywords for ISAKMP Versions 1.0 and 9.9 | IP, TCP, ISAKMP | IP Next Protocol = 6 <br> IP Source Address <br> IP Destination Address <br> TCP Source Port <br> TCP Destination Port |
