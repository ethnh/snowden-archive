# TLS trends at GCHQ 

![img-0.jpeg](img-0.jpeg)
# Source of data 

- Our TLS events come from our TLS app
- Runs on special source (approx. $200 \times 10 \mathrm{G}$ ) and Comsat data
- Produces unselected events: about 10 billion Server Hellos per week
- Records details about the handshake: IPs, Hello messages, Certificate, Key Exchanges
- Events stored for 6 months in our clouds
# Trends Reports 

- We summarise these events to produce weekly trends reports, which record:
- Types of key exchange (RSA/DH/EC)
- "Top 40" TLS services in use, highlighting new services and changes in existing services
- Details about the crypt (e.g. DH moduli)
- "Watchlist" to keep an eye on widely-used services (Facebook, Gmail, Hotmail, etc)
# Example: top 40 services 

## 41. Top Certificates seen by Common Name

| Common Name | Modulus | Valid From | Valid Until | Issuer org | Postion | \% of Total | Past \% | Raw Count |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| *. Facebook.com |  |  |  |  |  |  |  |  |
| xIMEL e. xiamat.net |  | 13/01/02 | 11/04/03 | BigCert. Inc. | 1 (1) | 6.381 (10.205) |  | 968772696 (3127416006) |
| www.facebook.com |  | 14/01/02 | 31/08/02 | GIC Corporation | 2 (2) | 7.005 (7.040) | **** | 802295227 (778478700) |
| ad. twitter.com |  | 17/11/02 | 13/07/02 | VeriStgn Trust Network | 3 (3) | 5.000 (5.443) |  | 521360555 (901320237) |
| *. hereall. com |  | 19/05/02 | 17/05/02 | VeriStgn. Inc. | 4 (4) | 4.440 (4.839) |  | 463021772 (524077717) |
| uts.microsort.com |  | 15/07/02 | 12/07/03 |  | 5 (5) | 2.720 (2.024) |  | 204450005 (200947521) |
| *. channel. Facebook.com |  | 16/05/02 | 15/05/02 |  | 6 (6) | 2.650 (2.504) |  | 270991437 (205510009) |
| s-statric.ak. ehodn.net |  | 23/11/02 | 26/11/03 | BigCert. Inc. | 7 (7) | 2.242 (2.401) |  | 253793075 (205510029) |
| m. Facebook. com |  | 26/11/03 | 26/11/03 | Akamai Technologies Inc. | 8 (10) | 2.180 (1.584) |  | 227502455 (575010529) |
| *. data.roplbae.yahoo.com |  | 01/08/02 | 01/08/02 | EcuFax | 9 (14) | 2.046 (1.520) |  | 213407210 (367941277) |
| logio.yahoo. com |  | 01/06/02 | 01/06/03 | EcuFax | 10 (11) | 1.757 (1.575) |  | 181117743 (375870821) |
| *. fo/man.com |  | 03/06/03 | 03/06/03 | BigCert. Inc. | 11 (17) | 1.710 (1.409) |  | 179150294 (315712115) |
| *. appgle.com |  | 03/06/03 | 02/08/03 | Entrust. Inc. | 12 (9) | 1.724 (1.751) |  | 178704944 (192002502) |
| *. www.updata.microsort.com |  | 02/08/02 | 02/08/02 | EcuFax | 13 (12) | 1.470 (1.342) |  | 154111650 (170445606) |
| s-statric.ak. Facebook.com |  | 08/03/03 | 08/03/03 | Google Inc. | 14 (15) | 1.390 (1.460) |  | 155141462 (302900355) |
| *. ad.loglo. top.net |  | 08/03/03 | 08/03/03 |  | 15 (12) | 1.252 (1.354) |  | 150543626 (340850541) |
| *. v.ty.manamore.com |  | 19/04/02 | 18/04/02 |  | 16 (35) | 1.180 (0.470) |  | 123301507 (52803604) |
| *. addong.mcyclia.org |  | 15/04/02 | 18/04/02 | Google Inc. | 17 (25) | 1.160 (0.650) |  | 100903041 (20099992) |
| *. secondend. com |  | 14/07/02 | 13/07/02 | VeriStgn. Inc. | 18 (27) | 1.094 (0.960) |  | 114150550 (506107305) |
| cbb.cymetew.hrf. prod.mlymea.net |  | 15/05/02 | 15/05/02 |  | 19 (20) |  |  |  |
| *. castle. zyngs. com |  | 05/05/02 | 05/05/02 | BigCert. Inc. | 20 (10) | 0.900 (1.120) |  | 59420796 (572110224) |
| *. ualendar.yahoo.com |  | 01/10/02 | 01/10/02 | Gedrrust. Inc. | 21 (20) | 0.955 (1.450) |  | 20100210 (214047140) |
|  |  | 05/08/02 | 05/08/02 | EcuFax | 22 (20) | 0.981 (0.907) |  | 90584855 (100277550) |
| *. Facebook.com |  | 04/08/02 | 04/08/02 | BigCert. Inc. | 23 (22) | 0.981 (1.125) |  | 97057311 (100474250) |
| *. v.ty.manamore. com |  | 04/10/02 | 04/10/02 |  | 24 (29) | 0.702 (0.584) |  | 75240341 (64223056) |
| *. v.ty.manamore. com |  | 01/10/02 | 01/10/02 |  | 25 (22) | 0.688 (0.739) |  | 71792445 (81745024) |
| *. v.ty.manamore. com |  | 06/10/02 | 06/10/02 |  | 26 (20) | 0.669 (0.614) |  | 69704602 (67057051) |
| *. v.ty.manamore. com |  | 07/10/02 | 07/10/02 |  | 27 (14) | 0.665 (0.730) |  | 69400948 (8156402) |
| *. v.ty.manamore. com |  | 08/10/02 | 08/10/02 |  | 28 (27) | 0.627 (0.627) |  | 65485931 (69559595) |
| *. v.ty.manamore. com |  | 09/10/02 | 09/10/02 |  | 29 (26) | 0.606 (0.650) |  | 65215855 (60000026) |
| *. v.ty.manamore. com |  | 01/10/02 | 01/10/02 | VeriStgn. Inc. | 30 (27) | 0.593 (0.651) |  | 60885989 (49001229) |
| *. v.ty.manamore. com |  | 01/10/02 | 01/10/02 |  | 31 (33) | 0.569 (0.521) |  | 59420796 (57769432) |
| *. v.ty.manamore. com |  | 01/10/02 | 01/10/02 | Gedrrust. Inc. | 32 (20) | 0.554 (0.775) |  | 57770165 (50023777) |
| *. v.ty.manamore. com |  | 02/10/02 | 02/10/02 | Thores, Inc. | 33 (42) | 0.530 (0.425) |  | 55267751 (49001081) |
| *. v.ty.manamore. com |  | 02/10/02 | 02/10/02 |  | 34 (24) | 0.514 (0.506) |  | 53094206 (55968031) |
| *. v.ty.manamore. com |  | 02/10/02 | 02/10/02 |  | 35 (38) | 0.509 (0.450) |  | 52084110 (49720507) |
| *. v.ty.manamore. com |  | 04/10/02 | 04/10/02 |  | 36 (21) | 0.492 (0.550) |  | 51395280 (50763021) |
| *. v.ty.manamore. com |  | 04/10/02 | 04/10/02 | Gedrrust. Inc. | 37 (22) | 0.470 (0.515) |  | 49056755 (15051007) |
| *. v.ty.manamore. com |  | 05/10/02 | 05/10/02 |  | 38 (20) | 0.444 (0.447) |  | 46310149 (49094909) |
| *. v.ty.manamore. com |  | 05/10/02 | 05/10/02 | Gedrrust. Inc. | 39 (44) | 0.430 (0.390) |  | 45721020 (43761751) |
| *. v.ty.manamore. com |  | 06/10/02 | 06/10/02 |  | 40 (43) | 0.413 (0.421) |  | 43796504 (46590125) |
| *. v.ty.manamore. com |  | 06/10/02 | 06/10/02 |  | 41 (62) | 0.405 (0.205) |  | 42322010 (22077002) |
# Trends Reports: Findings 

- RSA:DH:EC ratio roughly constant (90:5:5)
_ EC almost entirely Google (plus a bit of whatsapp)
- New certificates mostly use 2048-bit RSA keys
- We've seen new services jump up the list:
_ Summer 2011: Google's switch to Elliptic Curves
_ Autumn 2011: Apple's iCloud service
_ Spring 2012: Increase in mobile Facebook encryption
# TLS and targets 

- Trends reports not based on targeted data
- How do we judge interest in TLS services, and get analysts involved? Two ways we've tried:
- Associate TLS events with targets, and inform the relevant analysts (TargeTLS)
- Put TLS data out there for analysts to search (FLYING PIG)
# TSI/SI/REL 

## TargeTLS reports

- BROAD OAK: GCHQ's repository of target info
- We match TLS events against this:
- Is the server IP in BROAD OAK?
- Does the certificate's domain match a URL selector, or a number of email selectors?
- Email the relevant POC to ask if the traffic is of interest
- About 15\% of the services we've identified in this way have been worth looking into further
# FLYING PIG 

- TLS knowledge base. Summarises all TLS events to answer multiple questions, e.g.:
- What certificates are present on a given IP?
- Which client IPs access a given service?
- Which TDIs can be associated with a given service?
# Example: search by domain 

## FLYING PIG

## TL: 51/55 L. KN: 13 W L.C. CAE: $E$ A S: $C$

## HRS Fortification Query FLYING PIG - general SSL toolkit Query QUICK ANT - Tor everts Q7D

Query FLYING PIG
D) / network / certificate field /tomal ru
Query on $\square$ Client IP $\square$ Server IP $\square$ Bnth
or $\square$ fortrunk [e.g. 1.2.3.1|S7]
or $\bigcirc$ Server Certificate [e.g. Sunsimple.com (use \% for wildcards))
Run Query

## CORRELSE TROF ONTOC: 5/10/20

## AS HTTP requests matching your query ( $?$ (,

![img-1.jpeg](img-1.jpeg)

Tip 1: Right disk on a row to find all server IPs that serve that certificate!
Tip 2: Disk on the disk (on or the title bar to download data in C99 format)
Tip 3: Double-click on a field to enable copy and paste!
Tip 4: Chewgn displayed columns ('knots' is default; Advanced' adds R50 Modulus and rather suite distribution columns); Aasia columns (1 Advanced columns)

| 1 - 10 of 70 items |  |  |  |  |  | 10 | 125 | 150 | 1100 |  |  |  |  |  | 123 | 4567 | 44 |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| Full <br> Certificate | First seen | Last seen | Count <br> in $/ \mathrm{n}$ <br> 25th <br> Nov | Count all <br> time | Valid from | Valid to | Subject common <br> name | Subject <br> country | Subject org <br> some | 1ssuer common <br> name | 1ssuer <br> country | 1ssuer org <br> name | Self <br> signs |  |  |  |
| 300203:2030320011-05-22 | 2011-11-25 | 2082726 | 16633953 | 2011-01-31 | 2012-03-27 |  |  |  |  |  |  |  |  |  |  |  |
| 13:17:22 | 18:21:59 |  |  | 00:00:00 |  |  |  |  |  |  |  |  |  |  |  |  |
| 30520351209202011-09-22 | 2011-11-25 | 249926 | 1029292 | 2012-01-21 | 2011-02-22 |  |  |  |  |  |  |  |  |  |  |  |
| 14:03:50 | 10:53:22 |  |  | 00:00:00 |  |  |  |  |  |  |  |  |  |  |  |  |
| 20:00:00 |  |  |  | 23:59:59 |  |  |  |  |  |  |  |  |  |  |  |  |
| 20320323308202011-12-07 | 2011-11-25 | 10020 | 32820 | 2011-09-25 | 2013-11-28 |  |  |  |  |  |  |  |  |  |  |  |
| 20:03:55 | 10:53:49 |  |  | 00:00:00 | 23:59:59 |  |  |  |  |  |  |  |  |  |  |  |
| 303203231309202011-03-23 | 2011-11-25 | 676 | 9517 | 2010-01-25 | 2012-01-27 |  |  |  |  |  |  |  |  |  |  |  |
| 17:01:09 | 10:40:03 |  |  | 12:42:03 | 18:12:09 |  |  |  |  |  |  |  |  |  |  |  |
| 30520351209202011-03-22 | 2011-04-06 | 0 | 1402 | 2011-03-04 | 2012-03-05 |  |  |  |  |  |  |  |  |  |  |  |
| 08:14:31 | 00:15:55 |  |  | 06:42:12 | 06:42:13 |  |  |  |  |  |  |  |  |  |  |  |
| 30020425209202011-10-17 | 2011-11-25 | 22 | 1226 | 2011-05-27 | 2012-07-25 |  |  |  |  |  |  |  |  |  |  |  |
| 14:03:52 | 10:52:10 |  |  | 00:00:00 | 23:59:59 |  |  |  |  |  |  |  |  |  |  |  |
| 30020354308202011-10-09 | 2011-11-25 | 30 | 1150 | 2010-02-13 | 2012-11-00 |  |  |  |  |  |  |  |  |  |  |  |
| 00:03:03 | 17:04:02 |  |  | 14:19:06 | 14:19:06 |  |  |  |  |  |  |  |  |  |  |  |
| 30020415209202011-11-01 | 2011-11-25 | 246 | 692 | 2011-09-15 | 2012-09-14 |  |  |  |  |  |  |  |  |  |  |  |
| 07:00:59 | 14:25:29 |  |  | 11:47:51 | 11:47:51 |  |  |  |  |  |  |  |  |  |  |  |
| 30020254309202011-10-14 | 2011-11-21 | 201 | 326 | 2011-10-05 | 2014-10-04 |  |  |  |  |  |  |  |  |  |  |  |
| 10:00:04 | 10:00:04 |  |  | 00:07:04 | 00:07:04 |  |  |  |  |  |  |  |  |  |  |  |
| 30520415209202011-10-21 | 2011-11-25 | 99 | 259 | 2011-09-15 | 2012-09-14 |  |  |  |  |  |  |  |  |  |  |  |
| 14:14:18 | 15:45:50 |  |  | 11:47:51 | 11:47:51 |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |

## TS/SI/REL
# Example: search by server 

## FLYING PIG

## LESIS BL KNOWLEDGE BASE

HIS justification. Query FLYING PIG - personal SSL toolkit. Query QUICK ANI - for events CPE

Query FLYING PIG
IP / network / certificate field
Quary 22-73 Client IP Server IP ( 7 Both
or 13 network [e.g. 12.2.0/24]
or 1. Server Certificate [e.g. %example.com (use \% for wikipards)] Run Query
![img-2.jpeg](img-2.jpeg)
# TIS/ISI/REL 

## Contacts

- TLS trends: Crypt Operations BULLRUN team
![img-3.jpeg](img-3.jpeg)
- FLYING PIG: ICTR Network Exploitation
![img-4.jpeg](img-4.jpeg)
(@gchq)
