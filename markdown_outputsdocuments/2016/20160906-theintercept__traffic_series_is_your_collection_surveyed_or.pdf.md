# DYNAMIC PAGE -- HIGHEST POSSIBLE CLASSIFICATION IS TOP SECRET // SI / TK // REL TO USA AUS CAN GBR NZL 

## (U//FOUO) Traffic Series: Is Your Collection Surveyed or Sustained?

FROM: CSRC/Integrated Collection Strategies (S342), and
Menwith Hill Station, Analytic Discovery Division
(F77O15)
Run Date: 04/22/2009
(U//FOUO) Editor's note: Analysts, here's part 3 in our 5-part series with tips on how to get the best traffic...
(S//SI//REL) How often do you look at the case notation (CASN) and PDDG/SIGAD fields in your signal-related information (SRI)*? Do you know what they mean? Keeping track of the CASNs and FORNSAT collection sites for your traffic will help you optimize collection of your target's traffic; it can also alert you when you've been the happy recipient of traffic collected by another TOPI's sponsored collection requirement number (CRN) or a FORNSAT site's satellite survey activities.

## (U//FOUO) Sustained Collection vs. Surveyed Collection:

(TS//SI//REL) Traffic is collected in two ways: sustained tasking through CRNs entered into SURREY (as was already discussed earlier this week), and by ad hoc surveyed collection performed by a FORNSAT site's collectors. Each FORNSAT Collection site is responsible for collection of one or more satellites as dictated by their location in a satellite's footprint/beam. While FORNSAT collection sites perform sustained collection of satellite links tasked with CRNs, they also perform self-driven surveys of the satellites for which they are responsible in efforts to map and understand the site's collectable environment and identify new target technologies.
(TS//SI//REL) For example, MHS's MOONPENNY is responsible for 46 unique satellites. Of those, MOONPENNY is tasked to provide sustained collection on 163 unique satellite links/CASNs via SURREY CRNs. Between 1 January and 28 February 2009, MHS updated/entered 2975 CASNs in ROADBED. Of those CASNs, 112 were sustained; the 2863 remaining updates were from surveys performed by the collection site.
(TS//SI//REL) If you see a spike in your traffic, or if your traffic is coming in sporadically, FORNSAT surveys might be the reason. Consider this:
Unbeknownst to you, a FORNSAT collection site decides to spend a week surveying all the links on one particular satellite in its area of responsibility (AOR). You arrive at work on Monday morning to see that your target's communications have doubled or tripled in volume! Not only that, the traffic has more intelligence value than any you've seen before. You may think, "Wow, my targets have really ramped up operations." Then just as quickly it's gone -- your traffic is back to its usual level.
(S//SI//REL) What happened? Did your target really slow its activity? Have you upset the Traffic Fairies? No. The most likely answer is that the FORNSAT collection site responsible for that link has moved on. Unless you tell them you need that link collected through a CRN, your traffic will be lost. Noting the CASN in your traffic's SRI will help you determine whether your traffic came from a sustained CRN or a survey.
(S//SI//REL) What's in a case notation? How can you tell if a CASN is from a survey or sustained collection? Easy -- you can tell if your link was collected on survey or sustained collection just by looking at it. Here's how it breaks out:
(S//SI//REL) FORNSAT Discipline Survey CASN:
3BV1256832400000
The first two letters/numbers are the satellite digraph. (You can find a list of all the satellites and their digraphs in the Query section of ROADBED.) In this case, 3B tells us that the satellite collecting this traffic is Atlantic Bird 1. The third position of a FORNSAT survey notation will always be an H , $\mathrm{L}, \mathrm{R}$, or V . This indicates the polarization, and stands for horizontal linear, left-hand circular, right-hand circular, or vertical linear polarization. The series of numbers that follow show the frequency of the link/carrier. In this case, the carrier is on $12,568.324 \mathrm{MHz}$. FORNSAT survey CASNs provide you all the information you need for entering your sustained collection requirement in SURREY.
(S//SI//REL) FORNSAT Sustained Collection CASN: 3BBAC A case notation that is on sustained collection will consist of five letters or numbers. Here 3B still indicates the Atlantic Bird 1 satellite. The three remaining characters are arbitrarily assigned and provide no significant information, other than to make it easy to tell that it's a sustained collection CASN.
(S//SI//REL) Here is what the information would look like in ROADBED:

| Satellite | ATLANTIC BIRD $1 \mid 3 \mathrm{~B} \mid 347.5 \mid 27508$ |
| :-- | :-- |
| Frequency (MHz) | 12568.324 |
| Polarization | VER |
| Direction | DOWN |
| Priority | MISSION TASKED |
| Status | ACTIVE |
| Case Notation | Survey: 3BV125683240000 <br> Collection: 3BBAC |
| Site | MHS [USJ-759] |

(S//SI//REL) Armed with this information, you can assess the value of the data you're getting from a CASN and FORNSAT collection site to decide whether or not to enter your own CRN for sustained collection in

SURREY. (In the examples above, the information derived from CASN 3BV1256832400000 was used to enter a sustained collection requirement, with a sustained CASN of 3BBAC.) This information may also help you discover what happened if your traffic decreases in volume or disappears altogether, or if you should edit or cancel a CRN that you already sponsor.
(S//SI//REL) To learn more about entering CRNs and tasking FORNSAT collection sites, check out tomorrow's installment.
(U) Note:

* (S//SI//REL) It is important to understand the difference between signalrelated information (SRI) and metadata. In a nutshell, SRI is information about how the traffic was collected by a collection site; metadata is information about where the traffic actually came from and/or its intended destination.
(S//SI//REL) Signal-related information usually includes information such as dates, times, phone numbers, frequencies, transmission modes, etc. plus protocol information such as IP addresses, port numbers, etc. as well as additional information retrieved from the data itself. It generally describes how an entity is communicating, but does not describe the actual content of the message.
(S//REL) Signal-related information (SRI) is generated at the "front-end" of the SIGINT process -- from the collection source. [source: Signal-related information on WikiInfo]
(S//SI//REL) In the SIGINT environment, we generally take [metadata] to mean the information contained in and associated with a communication to identify, describe, manage, or route that communication, but not the information which could reveal the purport of that communication, or the whole or any part of the content.
(S//SI//REL) For COMINT, examples of metadata would be e-mail addresses, names, IP addresses, chat handles, transmission frequencies, telephone numbers, carrier IDs, Ethernet MAC addresses, data rates etc. The formal, legal, definitions of what constitutes metadata vary in detail across the Second Party partners, although the underlying intent remains consistent. -- [source: the COMINT Metadata Analysis WikiInfo].
