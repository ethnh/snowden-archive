# Mobile Apps - Checkpoint meeting Archives 

From GCWiki
Jump to: navigation, search
![img-0.jpeg](img-0.jpeg)
# Contents 

- 122 Feb 2011
- 28 Feb 2011 Project Checkpoint
- 325 Jan 2011 Project Checkpoint
- 411 Jan 2011 Project Checkpoint
- 530 Nov 2010 Project Checkpoint
- 62 Nov 2010 Project Checkpoint
- 718 Oct 2010 Project Checkpoint
- 85 Oct 2010 Project Checkpoint
- 921 Sept 2010 Project Checkpoint
- 107 Sept 2010 Project Checkpoint
- 1124 August 2010 Project Checkpoint
- 1210 August 2010 Project Checkpoint
- 1327 July 2010 Project Checkpoint
- 1413 July 2010 Project Checkpoint
- 1522 June 2010 Project Checkpoint
- 168 June 2010 Project Checkpoint - Status Summary (Updated 14 June)
- 1725 May Project Checkpoint
- 1811 May 2010 Project Checkpoint
- 1927 April 2010 Project Checkpoint
- 2030 March 2010 Project Checkpoint
- 2116 March 2010 Project Checkpoint
- 221 March 2010 Project Checkpoint
- 2316 February 2010 Project Checkpoint
- 242 February 2010 Project Checkpoint
- 2514 December 2009
- 267 December 2009
- 2730 November 2009


## [edit] 22 Feb 2011

## Present:

## PROCEDURES

Mobile TERRAIN

- Yahoo protocol change confirmed - App no longer able to process it.
- Tunnel timeout fix unproven. Evaluation awaiting restoration of service.
- Survey enhancement - in TERRAIN 10.5, comprises additional logging. to evaluate.
- Feedback mechanism for issues found during Mobile IV\&V was discussed. Feedback to TPS to be informal: TPS will raise internal tasks as necessary, will then track via weekly internal reports. Service Desk will not be necessary.
- The recent security incident, in which PDDGs, SIGADs and protective markings were wrongly configured, highlights the
need for formal system ownership and support. Current MVR HB planning indicates that Mobile TERRAIN will be needed for at least 8 months and probably longer. The PRESTON rollout process by TFE was discussed, using a test system, local file storage and check sheets before rolling out live. Training on Mobile TERRAIN config/support is being updated and will be rolled out to COMSAT sites by end of March.

- 10.5 build finalised today - last of the backports from 10.6.
- 10.6 includes App IDs as used by XKEYSCORE. Being upgraded to 64-bit RHEL5. APPId did not make it into 10.6. Problems with it crashing when ran on Redhat 5. We will be putting this into the first 10.8 build (mid March). [Updated]
- Flexilogs are showing performance \& complexity issues. $\square$ following up.
- TDIs also included in 10.6, except they have just changed to a different format, so capability for 10.6 is to be revisited (old, new, or none) - $\square$ to follow up. TDI's in Begal in 10.6. We decided to go with the latest Begal engine and therefore this will work with the latest GTE TDI's no issue. [Updated]
- Question raised as to whether GRX tunnels might enhance TDI convergence. $\square$ to investigate as a quick win for Surge Phase 1 .


# New Apps 

- Orkut, Bebo first drops and MySpace final drops now on Agility trial. A problem with MySpace is being investigated.
- Orkut, Bebo: Events PC currently cutting code around delivered App, in the absence of any defined requirement. Feature requirements still need defining. $\square$ to progress.
- Final drops now on for facebook, eBuddy, MySpace, ICQ, LinkedIn. $\square$ to verify/validate - starting with LinkedIn
- Nimbuzz, Whatsapp still awaiting XMPP progress. $\square$ to chase task via $\square$
- Legals still to be chased down.
- $\square$ to own OPS Explore phase of MVR rollout. $\square$ to advise $\square$ when apps move across to Explore.

TDIs

- TDIs for HB15: $\square$ has a list of ca. 20. These may need to be prioritised, typically for those which give Convergence. Currently GTE prioritise TDIs. Theme need to take over prioritisation of Mobile.
- $\square$ taking over TDI work from $\square$ in April.


## [edit] 8 Feb 2011 Project Checkpoint

Present: $\square$

## Mobile TERRAIN

- Content is only being seen for BlackBerry. Gmail is known to be encrypted. Yahoo has a suspected protocol change (being investigated), lack of Hotmail content remains unaccounted for. $\square$ suggested that the fix would hopefully require only a patch to TAMING PASTRIES.
- Tunnel timeout fix is expected to increase convergence rates to ca. 50\%. Rolled out to Benhall. $\square$ to pursue rollout at other sites.
- Survey enhancement. $\square$ to clarify usage.
- Coco01 (Bude) protective markings incorrectly configured. $\square$ suggested the signal provider should provide the classification at the same time as providing the signal. $\square$ said that the Mobile Access Lead $\square$ could take on this responsibility. $\square$ to talk to $\square$


## New Apps

- Facebook: TERRAIN 10.5 should produce about $50 \%$ of traffic types. $\square$ to clarify whether any of these are Content.
- Fring: expected to be ready for Experiment in ca. 1 wk ( 15 Feb ).
- Feature elaboration should be taken to the same level on both MVR and Mobile TERRAIN. Testing to the full level of detail, e.g. comparing the two platforms, is a big overhead.

Business benefits

- $\square$ reported that Convergence from a Bebo hit had allowed discovery of the PSTN for a Priority 1 target. Further C2C selectors had followed.
- $\square$ explained the urgent need to demonstrate further value to the business, and requested collection statistics. $\square$ to follow up.
- The focus for the demonstration was discussed. $\square$ requested TDIs. $\square$ explained the recent Project need to focus on MILKWHITE apps in MVR Experiment.
- $\square$ reported that the low volume of Mobile TDIs seen in Survey was due to GTE rolling them out to only four probes. Although Project does not have the resources to hand-hold the TDI business, $\square$ is pushing for wider deployment. This should resolve our inability to test/approve/deploy them to MVR.


# QFDs 

- SOC ANTH: Gb context: awaiting decision from OPS on how to handle bearer type display - may be sufficient to display the SIGAD.
- SOC ANTH: GTP CAID issue. Events from Mobile TERRAIN are OK, so it is an MVR issue. Workaround should be in place to allow re-enabling in SOC ANTH tomorrow ( 9 Nov).
- 3 x GMM event types being promoted to INTEGER SPIN. This should bring a Convergence benefit.
- OpEval availability - 2 weeks' time ( 22 Feb) suggested but unconfirmed.


## [edit] 25 Jan 2011 Project Checkpoint

## Present:

The meeting covered a lot of ground. Points are grouped by topic, not in order discussed.

## General

- OpEval is awaiting return of the upgraded Evolved MUTANT BROTH (This will not include the Context store which provides GTP convergence capability)
- Important that the Opeval is used to demonstrate business realisation against Mobile Network traffic.


## Traffic and survey

- Currently approx 12 bearers on cover, two more expected at Bude when coco02 is commissioned.
- Early reports from analysts suggest that significant quality traffic is being collected from Leckwith.
- Reference data from GMM on MVR is providing millions of hits into INTEGER SPIN (the QFD formerly known as Evolved GEO FUSION), with thousands of new cells identified. Geo GMM capability destined for Marbled Geko is being built as a demonstrator within Blackhole. Project to monitor.
- OPSD survey work is ongoing, led by The PPF Survey module is to be installed in MVR Experiment.
- Surveys indicate that $10 \%$ of traffic is BlackBerry, yet our intercept is $80 \%$ BB. The shortfall in expected webmail could have may causes. Investigations are being led by May need to call on TPS to conduct tests, although processing is not a strong suspect.


## Convergence

- Main problem at the moment is poor ratio of convergence, at 5\% of tunnel setups being identified. Experiments indicate that a tunnel timeout fix in TERRAIN will improve this to $50 \%$. Scheduled for TERRAIN 10.5. asked if this can be pulled forward in time for OpEval, possibly via an update to TERRAIN 10.5. to follow up.
- Further improvement would need a more complex tipping architecture. to follow up.
- QFD convergence upgrade - HA, eMB + Context store, has slipped to March. Plan is being agreed with NGE SU.

MVR processing

- GTP in-tunnel processing on MVR due in Experiment shortly. to provide update. Op rollout tentatively suggested for HB18, i.e. Autumn 2011.This would represent a substantial delay over previous estimates and would have consequences for supporting SA Terrain. to follow up.

New Apps

- Theme reported that Events they had seen in databases did not fully match the Events they had expected. Theme and TPS are working together to ensure alignment.
- Currently we cannot identify Mobile source for webmail (except Yahoo). Actor-Action ICD Version 2 will improve our ability to recognise traffic originating from a mobile device.
- Legal assurance for new Event types - now believed to be good. is setting up a meeting between Events PC and OPP-LEG to confirm legalities.
- MES apps on target for Experiment - risks with mail.ru, XMPP (Nimbuzz \& Whatsapp): these are not expected to differ
from the non-mobile versions, but confirmation is coming too late to fix them if anything does show up. $\square$ is following up with the Suppliers.

- Mail.ru delayed by lack of a linguist. Now sorted.
- Nimbuzz delayed by service account setup complications.
- Orkut, Bebo feature lists being developed by GTE Tracking team. Due to overlapping timeframes, there is no guarantee of delivered feature alignment. $\square$ to update feature list.

TDIs

- 13 now operational, 8 due in HB13, 8 more failed HB13 testing - to be investigated.
- $\square$ explained concerns that suitable bearers for TDI validation are not being chosen, leading to high rejection rate (not just a Mobile problem). $\square$ is pursuing.
- $\square$ stressed the importance of TDIs in informing new app selection.
- $\square$ reported that TDI rollout has been much streamlined. $\square$ felt that the benefits will not be felt immediately, until GTE can develop fast enough.
- New TDIs are expected to exploit the leaky app/gateway capability currently being built into the QFDs.
- TDI capability in Mobile TERRAIN is due in TERRAIN 10.6.
- Need to evaluate Terrain Ident Capability - separate to TDIs.

FY2011-12 reorganisation

- The business is recognising the scale and complexity of Mobile app development. $\square$ stressed the need to demonstrate associated benefits, and the need for it to become BAU: this will support an increase in business priority for Mobile. The wiki is an important tool in communicating process and progress. $\square$ to follow up.
- The business is looking at overlaps between Mobile and MTI work. A key difference has been Mobile's need for more rigorous testing. The relative states of Mobile vs. MTI test regimes were discussed. Agreement between Mobile and MTI is needed.
- The Mobile Surge arises from a FTCG finding that the business needs to do more Mobile. It will choose a specific piece of work across the business and focus on delivering a specific outcome, without putting additional pressure on known bottleneck areas. The aim is to prove the business benefits of Mobile.


# [edit] 11 Jan 2011 Project Checkpoint 

Present: $\square$
MVR

- HB13 MVR testing currently unable to verify some mobile TDIs due to lack of traffic. Need to ensure that suitable Mobile bearers are tasked for these tests. $\square$ is progressing.
- Value of getting TRAFFICMASTER into MVR Agility experiment was stressed. $\square$ to gain agreement from TPS and raise RFCs as necessary.
- Fring is last remaining app from July'10 tranche still to go on Agility trial. It requires promotion to TERRAIN. $\square$ discussing with TPS later today.
- Operational-standard GTP module is needed for the Survey MVR system. $\square$ has raised this with $\square$

QFDs

- HARD ASSOC and Evolved MUTANT BROTH both now risk slipping to February.


## [edit] 30 Nov 2010 Project Checkpoint

Present: $\square$

Agility and development

- All required handsets are now available.
- EAP (MIRTF) back on course: both PPF Apps and TERRAIN prefer this over Lawful Intercept as the strategic solution to app characterisation.
- Approach continues to be OPS led for requirements and technically informed. New apps ( bebo \& Orkut) to satisfy MES deadlines not ideal pragmatic in circumstance.
- GTE will be doing more up front analysis in the future to support feature requirements.
- Tunnel timeouts: experiment running on bostrom - timeout extended to 1 hr .
- 1 webmail hit seen to date. TND unpacking still being checked.
- It will be useful to compare MVR output with Mobile TERRAIN, to validate processing once MVR has GTP processing.
- Agility Trial needs to draw in OPS engagement for evaluating new app exploits. This should help provide leverage for getting the apps into HBs as well as supporting the Business change aspects.

New Apps delivery

- HB 12 is delivering MMS \& GMM Content as well as Events
- GMMaps: unselected content needs viewing restrictions in place downstream (being done). Two formats for Lat/Long have been found, which may mean that the HB 12 delivery will be incomplete. to check whether individual content types can be turned off.
- MMS is now tested and proven.
- Nimbuzz and Whatssapp use XMPP protocol, already being delivered under SINO Theme. These apps will be included in the XMPP delivery. Funding for Oct '10 tranche will transferred to SINO reducing MES forecast. Orkut and Bebo late replacements for Shmessenger and to increase funding profile. Suppliers can do the feature analysis. We will still need to capture details of the Event and Content types to be generated once PRDs have been provided.
- TPS will be moving their app feature records from VDD to a new system based on XML schemas. This is not scheduled but is expected to be in place by the end of 2010.
- App delivery timescales between MIP-3 vs. 4 into HBs and Terrain builds are subject to change.
- Critical to get July'10 and Oct'10 apps onto Agility Trial by end of the FY (March 2011).


# MIP-3 \& 4 

- MVR GTP expected in experiment space in Jan 11
- TERRAIN 10.4: no benefit to Mobile for MIP-3. 10.5 will deliver benefits for MIP-4.
- Content delivery will focus on content we can already visualise.
- Also need to develop new content types along with refining the approach (e.g. to make better use of Open Source file viewers).
- Unselected content issues need better visibility to developers: New Traffic Types needed.
- Mobile TDIs deployed for MIP-4 unlikely to hit the 100 mark.
- P6 to be updated for MIPs $3 \& 4$


## [edit] 2 Nov 2010 Project Checkpoint

Present:
Focus of the meeting was on the MVR Heartbeat 12 release and New App capability.
Initial apps

- GMMaps: HB12 expected to process all 12 traffic features (Terrain 10.3 restricted to 2 features). All will be promoted to BLACK HOLE and SILVER LINING. Downstream design pending legal decision on what can be passed to which QFDs.
- MMS: HB12 is providing events although suggestion that content promotion should be also be available. Action to clarify.
- Hotmail: HB12 will include the protocol update. Such updates do not normally add new features. This one doesn't.

July 10 apps (MES)

- None of these will include Windows based Mobile Phones by design, though some may be compatible.
- Facebook: 1st drop (Login only) received. 2nd drop also, but unconfirmed. 3rd drop expected 3/11. to follow up. Project will seek to update Agility trial with latest available. From drop 2 on, the implementation rolls desktop and mobile into a single app, so it is unlikely that we will be able to tell which user client was used.
- ICQ: PRD-2 outstanding. Action to chase.
- MySpace: PRD2 just arrived.
- Fring: due to need for TERRAIN session processing, this is being developed in-house. Awaiting TERRAIN capability may be available to install onto Experiment agility. Action to check.
- eBuddy. This release to exploit IM only. To be delivered in a single drop, due 3 Dec.

Oct 10 apps (MES)
- Nimbuzz: PRD-2 due mid-Nov.
- WhatsApp: PRD-2 due mid-Nov.
- LinkedIn: PRD-2 due 3rd Dec.
- Mail.ru: complex delivery which hooks into two other tasks.
- Shmessenger: Based on WAP/jabber type protocols, so may not be accessible via our current handsets. Detica to investigate feasibility. If feasible, PRD-2 due mid-Nov. Agreement that we go ahead with analysis with Detica. GTE findings also to be made available.

TDIs

- Contractor access to TDI NOCON information resolved: will require signing an NDA - PoC is $\square$. Request has now been raised.
- 40 to go in HB12. $\square$ to follow up No. of Mobile TDIs in this drop.

Characterisation environments:

- Pivotal role of TPS in comms between OPS and Suppliers was stressed to support traffic sample collection using unattributable phones. Comms are now improving.
- $\square$ to check whether suppliers have full set of Lawful Intercept devices each, including Windows.
- $\square$ is reluctant to use the Mobile IRTF (EAP) for July Apps \& Oct Apps, because it represents a new way of working. Agreement that Legal Intercept will be used to collect samples. $\square$ is PoG.

Other

- Tunnel timeout during processing: $\square$ is pursuing.
- Ability to distinguish between mobile and desktop versions will be implemented in AA format version 2, expected Feb-Mar 2011. To take advantage of this, any given App will need to be updated.
- Mobile GTP Experiment Agility Trial will be used for quick evaluation of new software drops. It will not be used for formal testing.
- Jan 11 apps: list to await outcome of December budget/portfolio review.


# [edit] 18 Oct 2010 Project Checkpoint 

Present: $\square$

Agile development

- The Mobile IRTF (EAP) SyOPs is nearing a state at which it can be circulated to GREENHEART for comment/approval. The need to fit with GREENHEART's normal business activity was stressed, and any use within sensitive sites ruled out.

Bearer tasking

- At this moment EREPO is the only GRX feed still tasked. $\square$ is seeking to speed up the process for new/replacement tasking.

Infrastructure

- MAGLITE is delivering IOC capability for: EREPO, Bude (Gn and Gp) processing. Mobile Apps Project approach is then to improve exploitation of apps and associated convergence.

New Apps

- Google Maps legals to be cross-referenced with events being generated. This will be used to inform downstream, to ensure legal compliance.
- Facebook initial drop is in TERRAIN 10.3 and contains limited capability but should include convergence data.
- $\square$ has provided a detailed breakdown of New App expected features and event/content types. TPS have received asks from other areas, stretching resources - e.g. IM and VoIP are done in-house and resources are barely sufficient to deliver IM asks alone. Prioritisation will be necessary. To help prioritise, Theme needs visibility of projected costs per feature. $\square$ to keep Project informed of actual event/content types to be delivered by each TERRAIN rollout.

Processing

- TERRAIN 10.3.7 soak tested on bostrom. Lone dhelix error identified as caused by unexpected data type: no further
instances seen. This version will roll into MVR heartbeat 11.

- TERRAIN 10.3.8 includes new Hotmail protocol. Will shortly start soak testing at Bude. This version will roll out to PRESTON, Mobile, SMO. PoC for SMO schedule is $\square$ To gain visibility of Mobile benefit, Project will work with $\square$ to engage MELs.
- TERRAIN 10.4 is mopping up changes that were missed for 10.3 .
- 6x Mobile TDIs expected in HB11
- BEGAL processes TDIs within the PPF. Work under way to create an OS-independent version compatible with standalone TERRAIN. For commercial reasons, TDIs are classified TSS2 NOCON - this makes life complicated. TERRAIN 10.6 will provide TDI capability.


# [edit] 5 Oct 2010 Project Checkpoint 

Present: $\square$

## Survey

- TDI progress needs clarifying. $\square$ to speak to $\square$ and others in OPS.

Bearer tasking

- 271 has been providing traffic.
- SSOS have now tasked 040, 521, 099 and 072 to defined hosts - $\square$ imminently to configure DAG/TERRAIN processing.
- 032 via POKERFACE no longer required.
- BUDE-TAS still need more training on TERRAIN tasking/monitoring. $\square$ to go down and provide update to training team. $\square$ to obtain list of trainees and forward to $\square$

Processing

- We have no evidence that webmail is either working properly or not working: issues discussed included likely proportion of webmail in GRX traffic, lack of characterised light, lack of sufficient markers on records to identify collection source, immaturity of current data analysis tools. Neither PRESTON nor the EAP can deliver GTP stream format to allow processing to be confirmed.
- Significant RISK: IPP have no IA or proposals available for the July '10 apps, due to delay with Roke.
- Roke report availability problems with our handsets service to generate characterised data. We do not want this excuse to be available to them. $\square$ to pursue.

Repositories

- SOC ANTH improved version now in beta.
- Analysis would like clarification of Convergence QFDs. $\square$ to provide on wiki, on or linked from MIKC wiki pages.


## [edit] 21 Sept 2010 Project Checkpoint

Present: $\square$
Survey

- Survey tool to identify GTP/GRX in 10G's: RFC raised on Events PC, initial capability due for MIP-2.
- $\square$ to find out how many TDIs in the upcoming release are Mobile. [UPDATE: only one.]

New Apps

- $\square$ should be able to carry out end-to-end tests on webmails using PRESTON handsets, over the next few days. $\square$ to clarify current TERRAIN build for PRESTON. [UPDATE: An RFC would need raising to update the PRESTON Terrain build - 2 week delay. $\square$ is investigating with $\square$ whether the PRESTON data can be routed to BOSTROM.]
- MILKWHITE funding on July'10 and Oct'10 tranches is on target for financial accrual this FY, with apps in Experiment/Explore stage by then. First Facebook increment already received, with content appearing in TERRAIN
10.3 .

- Facebook Windows O/S handset was not available to be included as part of Roke proposal. Issue is being addressed PoC $\square$ (SSOS/SSE) is responsible for unattributable phones.

Tasking \& processing

- TERRAIN Support arrangements need strengthening. Current reliance on $\square$ (SSOS/SSE) for access to bearers. Business case for access to bearers via MIDDLESEX GREEN with PTC support. $\square$ (Mobile Access Lead) to coordinate access. TAS-Bude currently task bearers. TFE and TAS-Bude - tickets not being raised. TFE relationship to be clarified/strengthened.
- ACTION: $\square$ to seek formal approval for sustained tasking of 040, 271 and 521 via MIDDLESEX GREEN.
- Ownership of tasking incidents (e.g. loss of light) to be transferred to TAS-Bude. They have requested training in TERRAIN configuration. No training exists. $\square$ has some practical experience: $\square$ to investigate building training info on the wiki. Possible option is to revise tasking/support model.
- Urgent needs to: turn off BlackBerry processing and stop boxes crashing, move 040 to a functional TERRAIN. $\square$ is trying to find out how we can task Support to action.
- EREPO: Details of the MAGLITE sustainability uplift to be clarified with $\square$ to check with $\square$ and $\square$ whether dual-routing to Mobile Ref is acceptable.
- Agility trial can only be tasked with 4 bearers while in Experiment. Currently Convergence agility trial is tasked with 040 and 271. When it moves to Explore, more can be tasked - 12 to 20 bearers.

Processing architecture

- MVR will not provide full Mobile functionality for some time, i.e. GTP content no forecast date. Meanwhile (ca. 1yr) standalone TERRAIN will be used.
- $\square$ explained the differences in webmail processing by MVR (Generic Webmail Framework) and TERRAIN (TAMING PASTRIES). In due course these should merge into a common code base.


# Repositories 

- GMmaps processing is ready although full solution for downstream repository not expected.
- Not clear whether SOC ANTH can ingest all Facebook Events that will be generated. To be clarified.
- SOC ANTH - second instance due at Bude in 4-6wks. Queries will be federated across both SOC ANTH instances.


## [edit] 7 Sept 2010 Project Checkpoint

## Present:

## Project

- $\square$ presented his Action Plan to stabilise the deliverables for MIP-1, following the disappointing outcomes so far. These actions are necessary before we can move forward - a key objective is to demonstrate value to OPS and gain confidence in the approach. Two stability issues are critical to success: bearer tasking, and New App processing in TERRAIN. Other stability issues relate to DAG cards and EREPO.

Access and survey

- Despite some 900 10G bearers being accessible to GCHQ, their GTP potential is not clear. Only a handful of bearers are known to contain GTP, and tasking of these is unreliable. Project to engage with $\square$ to ensure adequate stability of feeds to enable Project to deliver benefits.


## Processing

- $\square$ is going to become tech director for TPS. As a consequence of this and other upcoming staff moves, TPS resourcing is likely to be an issue over the coming months.
- MVR Heartbeat 10 is coming under threat due to issues with new ENCHANTERSS functionality unrelated to Project needs.
- Project has closer control of the TPS TERRAIN processing stack, and so will focus on this as the only viable platform for current deliverables.
- $\square$ stated that TERRAIN is a better option for processing tunnelled traffic than PPF.
- TPS TERRAIN is now feeding SOCIAL ANTHROPOID: $\square$ to continue IV\&V investigations.
- Little Mobile App intercept has yet been seen. $\square$ to arrange for live input stream capture \& packet analysis, to confirm presence of Mobile App traffic.
- (update to Action 14/2): $\square$ to arrange cross-BU meeting (Apps/protocol analysis, Testing, CNE) to establish usage requirements for the EAP/LI and handsets.


# [edit] 24 August 2010 Project Checkpoint 

## Present: $\square$

Survey

- PPF GTP Survey - all but one field (DNS) already implemented, just not in expected format. Importance of this field to be evaluated. Aim to have pilot to be available by October (MIP-2)
- Approx. 30 TDIs are in the system to be developed by GTE. Not clear when this will be rolled out to MVR \& TERRAIN but may be available on Agility trial earlier.

## Tasking

- Bearers such as 271 and 040 remain under threat of de-tasking at any time. ACTION: $\square$ to present Business Case to board for retention of Mobile bearers.
- DAG card dropouts: $\square$ has asked for a Problem Ticket to be raised for the DAG solution.

Test systems

- $\square$ diagrams of the EAP and similar handset test systems.
- ACTION: $\square$ to arrange cross-BU (App/protocol analysis, Testing, CNE) meeting to establish usage requirements of the handset systems.
- Test processor system (bostrom) now running TERRAIN 10.2.5. BlackBerry decompression seen. Hotmail, Gmail not yet seen.
- $\square$ is having problems recording a sample of 271. ACTION: $\square$ to help facilitate recording of 271.

New Apps

- Google Maps legals now sorted. $\square$ to engage with TPS.
- Event and Content types being synchronised between App processing delivery and MVR Heartbeats
- "July 2010" App analyses due mid September. Might include early release of part functionality, which might then pull forward into MIP-2
- New CmR traceability ready for implementation on next ("October 2010") apps.
- 6 "October 2010" Apps (5 plus 1 spare) to be identified by Friday 27 Aug: Action on

Processing

- TPS TERRAIN to be upgraded to 10.2.8. Opeval will confirm whether Gmail \& Hotmail are working. $\square$ to provide definitive statement on Gmail \& Hotmail by next Checkpoint: Action on $\square$
- TPS TERRAIN: 3rd Line support $\square$ is overstretched. Training for DAG cards to be rolled out.
- MVR HB10 to deliver for core Internet only: MMS \& GMM Events, Hotmail, Gmail. $\square$ to follow up why no BlackBerry or Yahoo.
- MVR PPF promotion to TERRAIN to be resolved for MIP-3.
- Identification/watermarking of Mobile App intercept from core Internet is TBD. $\square$ stressed the importance for Convergence.


## Convergence

- SOCIAL ANTHROPOID UAT is imminent in the next few days.
- Event Unique ID (CAID) can now be used to correlate NGE Events with UDAQ Content (HAUSTORIUM does not do CAID).
- HAUSTORIUM decommissioning scheduled for October 2010. SALAMANCA to stay for a bit longer.


## [edit] 10 August 2010 Project Checkpoint
# Project 

- MIP-2 to focus on MVR processing, with New Mobile Apps capability being deployed against the core internet.
- Ownership of Business Change planning to be clarified.
- Identified uses of the EAP and related facilities include: TDI discovery, GTE quick look at new apps, IPP deeper look and new apps, IV\&V. Documented CONOP is required to clarify usage. This work is being actioned.


## Tasking

- Limited number of GRX bearers and lack of stability make it hard to demonstrate potential and hence obtain buy-in from the wider organisation. Survey work to date has been tactical and patchy. Quality of the toolset needs to be clarified. Need to engage
for access and survey support.


## New Apps

- 24 TDIs have been requested. Will take up to 6 wks to implement, though will be trialled in Agility before then. GTE can then survey, to inform next tranche of new apps.
- If needed sooner to maintain spend profile, will default to more webmail apps.
- Other possibilities include LinkedIn, iTunes, YouTube, although the ability of Content PC to ingest new formats will be limited.
- TPS-IPP, GTE, OPS roles becoming clearer, but still need Project to help define specific activities and ownerships. Action Mobile Theme to help facilitate clarification of roles.


## Processing

- BlackBerry, MMS operational. TERRAIN 10.2 expected to deliver Gmail \& Hotmail fixes, BlackBerry decompression, Yahoo mail.
- Bostrom test box has TERRAIN 10.2.5, awaiting to configure system.
- Gmail has all gone encrypted, so processing may not be possible .
- Hotmail service is undergoing transition to new design - may affect our ability to process.
- Emerging trend towards mobile devices, e.g. HTC Desire, spoofing fixed formats when connecting to app services. May need to review processing roadmap.


## Targeting

- First 10 TDIs due in TERRAIN 10.3.
- Mobile selector management for MVR is not so much a problem with TRAFFIC MASTER, as with the ability of BROADOAK, MONKEY PUZZLE, TACHO, etc. to ingest Mobile selectors.


## Convergence

- NGE are revisiting their roadmap and delivery schedule again. SOC ANTH likely to slip again, eMB and HA convergence work likely to slip beyond August.


## [edit] 27 July 2010 Project Checkpoint

Present: $\square$
Project

- MIP-1 impacted by further NGE delays. A second exception is being raised with delivery date now 25 Aug for Social Anthropoid.


## Tasking

- 3 new GRX ends, including both ends of 521, have been tasked. Data flow not yet confirmed, some issues with UDAQ.


## Processing

- TERRAIN 10.2.5 now on Test system (bostrom). Hopefully this will give us Gmail and Hotmail
- E2E testing held up until can fix one of the DAG cards.
- MVR Heartbeat 10: although GTP processing is being held back, expectation is that Mobile Apps should still roll out to
Core Internet. $\square$ has asked IPP for formal statement of Mobile features to be delivered.
New Apps

- Tranche 2 - Features all now with Industry. Facebook requirement now being considered by industry.
- Next set needs to kick off. $\square$ suggested that more mobile webmail would be valuable and easy, also perhaps restarting Viscom if it is visible in the new feeds.

Data characterisation

- We need characterised data to inform New App requirements as well as to inform testing. Project has incomplete technical knowledge of the facilities available. ACTION: $\square$ to pull together details of the technical capabilities/features of the EAP and other sources of characterised handset data.


# [edit] 13 July 2010 Project Checkpoint 

Present: $\square$
Project

- MIP-1 rescheduled for 30 July 2010
- There is a disconnection between Project needs and TPS delivery. $\square$ to update CmRs. $\square$ to update product database.

Processing

- PPF promotion to TERRAIN currently uses a temporary solution which could overwhelm TERRAIN. $\square$ to progress a long-term solution.
- TPS will produce Telephony Events in AA format for ingestion by the Events Buffer and subsequent passing to SALAMANCA or equivalent.

New Apps

- Action 04/6: Google Mobile Map Tile Events need to be defined. $\square$ requested that this Action be reworded accordingly.
- Tranche 2 App features to be defined this week by $\square$ can progress the preliminary analysis.
- Facebook and BlackBerry decompression are candidates for TERRAIN 10.3 - $\square$ to confirm status.
- ACTION: $\square$ to follow up Gmail decryption with ETPD


## [edit] 22 June 2010 Project Checkpoint

Present: $\square$
Project

- Directors Workbook Review (DWR) due 1 July.
- Checkpoint meetings moved to new dates/times, to avoid clash with Maglite checkpoint. Revised, more focused list of invitees.
- $\square$ is receiving stakeholder requests which need to be formally actioned. ACTION: $\square$ to call meeting to link stakeholder requests with change control.
- Operationally lots of queries being raised as MELs start to analyse GRX collection.

Enterprise Access Point

- Due to go online at end of June.

New Apps

- Google Mobile Maps: $\square$ to provide steer on legalities for Events vs. Content and consequent processing/storage of intercept. This is needed to inform planning.
- Analysis work by Ops/GTE/TPS to inform requirements is not formally controlled i.e. no forecast completion dates or formal dependency. ACTION: $\square$ to define cutoff date for initial analysis of the 5 second-tranche apps.
# Dataflow 

- Events for Hotmail and Gmail on Nokia \& iPhone will be forwarded via AA to NGE within HB8. These events will only be available via legacy events systems until Social Anthropoid is completed.


## Converged Events

- SOCIAL ANTHROPOID has slipped, pushing MIP-1 out of tolerance. Exception action underway with Project Board. Availability for UAT is now 30 July 2010.
- NGE plan currently has no milestone for SA UAT availability. Ideally we will link to this dependency milestone within P6.


## [edit] 8 June 2010 Project Checkpoint - Status Summary (Updated 14 June)

## Present:

Access

- Bearers being processed by ueda01:
- 040, 271 - routed via POKER FACE
- 044 - was expected to have disappeared but some intercept still arriving. to check.
- EREPO GAMMA - problems reported yesterday. [Update] have been asked to investigate.
- Bearers available on the OSDS:
- 035 (Saudi STM-16) - both ends.
- Other assorted single ends, to be confirmed.
- These should make up the 10 required for MIP-1.
- Survey tool - no formal contract placed: we have CmRs but have not levied them.


## Enterprise Access Point

- Wiring-up due over next week, first drop 18 June.
- TPS should by then have handsets and be able to run test scripts.


## Processing

- Demo of dual-DAG solution using STM-4 + STM-16 due this Thursday. sees no problems in migrating solution to dual STM-64 DAGs.
- Okada01 and 02 each have a single STM-64 DAG. [Updated] PO raised for Second card for each, plus two more for haga. Project Risk that the cards may arrive too late.
- There is a risk that TERRAIN may need changes for dual-DAG operation, and if so these may miss MIP-1.
- If the DAG solution fails, the fallback is to use POKER FACE.
- SIGADS and PDDGs now configured correctly, except that the SIGADs require a Z suffix for Mobile.
- Kato01 now has upgraded OS and OVO. All eight Ninjas should be upgraded over the next week or so. is aiming to get bearers connected up by then.

Test TERRAINs to miss v10.0 and go straight to an early drop of 10.1 .
New Apps

- Still need to confirm content processing for Gmail and Hotmail.


## Dataflow

- We are now seeing Mobile content in IIB.
- Routing requests for SAMALANCA, HAUSTORIUM and GDR (IIB) have gone in. Still to request full changes needed to route first to Dev systems, then migrate to Op. Operational data integrity still needs to verified into SALAMANCA and HAUSTORIUM from the output of Ueda 01.
- $\square$ says that the AA format is so different that data set comparison with legacy is not worth doing. will work with $\square$ to clarify way ahead.
- Currently formatting in CCDF v4.5. PCs will upgrade to 1.1.1 when systems are compatible.


## Converged Events

- Agility Trial is providing AA format to NGE (update - has moved from Dev to Op NGE Buffer)
- Issues over the ways that ENCHANTRESS vs. TERRAIN handle tunnel data are to be resolved.
- SOCIAL ANTHROPOID user base of ca. 20 is sufficient to meet MIP-1.

Sustainability

- SSOS access, Bude tasking, TFE 2/3rd line support, and GTE monitoring of POKER FACE, are providing adequate sustainability for MIP-1.
- $\quad$ is coordinating work elsewhere to improve GRX access. Project need visibility of this.

Beyond MIP-1

- Need to confirm dates for TERRAIN 10.1
- MAGLITE are pursuing GPRS selection for collection - currently still only $1 / 3$ turned on. Project to monitor this.
- Test handsets are making progress, the first few should soon be available to TPS/GTE. This will allow detailed specs on the next tranche of exploits to move forward. The process still needs to be formalised to be Ops-driven while technically informed. Meanwhile, $\square$ is working on research for Facebook and Twitter features.
- Bude infrastructure to be delivered for MIP-2.


# [edit] 25 May Project Checkpoint 

Present: $\square$
Project

- New Level 1 Milestone to be created, for agreement on Twitter and Facebook features to go in TERRAIN.
- POKER FACE now stable, with over a thousand Content hits in IIB. We are engaging the Analyst community to gain awareness and evaluate.


## TERRAIN

- Dual DAG card - demo scheduled for 10 June.
- Version 10.1 is available a month early. An interim 10.2 has been mooted, so the currently planned 10.2 may be redesignated as 10.3 .
- will work to link feature deliveries to requirements, and to clarify a pre-release build approach for the Test environment.


## Events

- $\square$ absence is holding up the Events L2 design.
- Converged Events in SOCIAL ANTHROPOID - timetable remains unclear. will continue to push for a date.
- ACTION: to check for Mobile Events in HAUSTORIUM \& IIB.


## [edit] 11 May 2010 Project Checkpoint

Present: $\square$
Access

- Three STM-64 single ends have been identified in the PEBBLE BED GPRS query. $\square$ to look for the other ends.
- GPRS selector management - the long-term solution for MONKEY PUZZLE and BROADOAK is being pursued by $\square$ $\square$ Meanwhile, $\square$ s working to get analysts to select it manually.


## Processing

- TERRAIN's May 15th level 1 Milestone for operational capability is at risk from issues over RHEL OS vs. OVO (system monitoring) version compatibility. Versions compatible with each other and with the TERRAIN apps are being sought.
- DAG card purchases for the TERRAINs are not visible. $\square$ to follow up.
- $\square$ confirmed that TERRAIN 10.0 will provide BlackBerry, MMS, Gmail and MS Hotmail Content and Events. Gmail/Hotmail Events will be Send and Read only.
- BlackBerry decompression will arrive in TERRAIN 10.2. There are advantages to early testing of a pre-release version in the Mobile Apps Ref environment.
- The issue of identifying mobile vs. Internet derived intercept was discussed. Any GRX metadata is discarded, so there is only the app session to go on. Hotmail processing can detect the mobile variant, but the Gmail processor cannot - we would need to look in the WAP, HTML, etc. metadata. Otherwise, in general we would expect the arrival of mobile capability to result in a step change in quantity.
- The next tranche of mobile apps has several candidate lists put forward by various sources. $\square$ is clear that the choice must be OPS' call, Project cannot second-guess.
- Lots of unprocessed binaries arrive in IIB. We need to push the re-entrant processing (agile development) environment, in order to explore it. This should help inform future new app decisions.
- HB 8 will deliver benefit for Mobile Apps - several webmail events and Gmail \& Hotmail content from within the core internet (outside the GTP tunnel). Detail to be added to project plan.


# [edit] 27 April 2010 Project Checkpoint 

## Present:

Scoping and requirements

- ACTION 6/1 (to ensure that users are looking at metrics): to work with to progress this.
- ACTION: to record requirement to target on GRPS selectors by default (Note this is distinct from Action 5/3 on to get users to set this option).
- User stories, data types and visualisation requirements are in hand. PoC

App Summaries

- Next tranche urgently needed if TPS are to be kept on side. Project may need to pick up and run with our own assessment of priorities and requirements and priorities. This is likely to focus on volume, in order to inform future decisions. Facebook is a strong candidate. ACTION: to raise urgency of App Summaries with next Tuesday.
- 10 is new PoC, alongside 10 has been standing in while 10 was away, she is not a poc. will speak to to get the proforma amended.
- Facebook, Fring and Nimbuzz placeholders created (Note: Facebook Summary has in fact been partially populated).

Light

- Mission Management of Benhall TERRAINS by Bude is now in place.
- Useful amount of traffic now present in feeds, to develop against.
- ACTION to push for movement on GTE Franchise. I think this related more to App Summaries, see note above.


## QFDs/Visualisation

- ACTION: 1000 o confirm that all parties have bee informed of the decision to dual-route data to both IIB/UDAQ and Golden Eye.
- Social Anthropoid rollout is tight. ACTION: to speak to 100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
- 5.3.3.1999 10:10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:10:10 10:
- Google Maps product is to be delivered in ADF format but wrapped in CCDF. Action to write up the agreed solution.

Databases and Analysis

- HARD ASSOC and evolved MUTANT BROTH are now running. Converged SOCIAL ANIMAL is awaited. Presentation now due ca. mid-March. Action 1/2 ( to discuss date) to remain open.
- Project is still aiming to implement AA ICD by May. Action to investigate if there is a risk associated with the delay to SOCIAL ANIMAL.
- Action 4/2 (analyst visualisation needs) dependent on 4/1 - update accordingly.
- TSPC2B 5 Eyes sharing solution will be dependent on the quality of the QFD content. Action on to register risk that: any slippage that impacts our end of June milestone will impact on TSPC2-B testing.
- Telephony Events destination/s need establishing. Action to clarify PPF Telephony Events routing/destinations with TPS and OPS.

Project

- Project planning to factor SMO Planning Agility Pilot. Action


# [edit] 16 February 2010 Project Checkpoint 

Access:

- GTE now able to survey the access environment for GTP traffic - whilst each bearer seems to carry relative low volume, this traffic is expected to increase and it is important that we can process it.

Processing:

- Converged Events pilot evaluation by IV\&V team is due by 28 Feb. NGE will be asked to provide a presentation and demonstrate the concept of converged comms events. Action to discuss date of presentation with Events. Breaking news - this work has slipped but is expected within 2-3 weeks.
- Content selection by ENCHANTRESS is not passing the IP and other outer layers to TERRAIN, which cannot then make associations. PoCs in TPS are and . Action (IPP) to raise report in shape of exception ie detailing problem and options. The 17 May delivery may be descoped although it appeared that Content may still be presented. Content obviously a key stakeholder for this issue.
- GOLDEN EYE II will take IIB flow from end of March (LOOKING GLASS will have partial capability by then).

App processing:

- The Data format issue was previously highlighted via Google Maps. GM also has a content issue. and are writing a Problem Statement - is chasing.
- PPF, SORCERER and TERRAIN have different requirements managers. The lead Product Centre must be the single PoC for the Project, and bring people together as needed.
- Dependencies lead each app through a cascade of product centres. Action to synchronise PC roadmaps.
- Viscom spec is awaiting completion of current traffic analysis.

Analysis:

- LOOKING GLASS developers in TDB need to understand the detailed requirement. Action to align analyst visualisation needs with data sources/formats, via pro-formas or similar.


## [edit] 2 February 2010 Project Checkpoint

- A Top Level Build Logic diagram for the next six months for the project is now available on the wiki.
- Three key delivery areas are currently Converged Events, 10GTP processing and Mobile Apps. Converged events are the critical dependency for QFD development and NGE showcase event.
- Key decisions on Converged Events Roadmap expected this week.
- The diagram highlights the need to roll out capability on TERRAIN as well as on MVR. has raised some new RFCs with IPP.
- New Apps:
- Mobile Gmail is currently not encrypted, but there is a risk that it will be in due course. New Risk to be added to GCrisk
- Hotmail analysis summary to be populated. Action $\square$ to chase.
- Google Mobile Maps: Content will require a new data model for the databases. Content will need data asap to develop this. Action TPS/Theme
- Viscom data poses compatibility issues with the ENCHANTRESS processing architecture. Existence of traffic also a risk. Activity in place to clarify priority and risks. New Risk to be added to GCrisk
- TDB content have provisioned effort to process the 5x Mobile Apps although Work Package required. Action
- to draft words for
- TDB content need to understand how the Apps content should be presented. Wiki Proformas should assist although direct engagement with TPS developers required. Action $\square$ to facilitate
- Access:
- The 10G GTP Pilot derisking exercise was successful, with the Level 1 milestone achieved. Report now published on Mob Apps Wiki.
- New workstream 13 initiated to improve access and provide sustained collection of GTP traffic.
- Business change: Planning is ongoing, with $\square$ ensuring a triangle of discussion between Theme, Ops and Product Centres.
- LOOKING GLASS will not be widely available for the Converged Events training in June - assumption is that training can still go ahead with direct QFD queries
- LOOKING GLASS will still need be available to selected analysts.
- $\square$ stated that current focus and testing scenarios are against available Mobile Internet traffic.
- Checkpoint Meeting aim is to monitor key deliveries ( and issues) leading up to key integration milestone (L0) in June 2010.


# [edit] 14 December 2009 

## Present:

- Business Change Dashboard being updated. To go on wiki when done and agreed by Principal User and Senior User.
- Mobile Theme Principal User, is likely to be moving on at a date to be agreed in the New Year.
- Programme understand the need to advise Thread mgt of any other products that would impact our portfolio of work.
- Pilot deliveries (GTP, Converged Events) are dependent on Product Centres delivering on time. These are being tracked/assessed.
- TERRAIN output via the new ICD is expected this week.
- Scope creep is occurring over pilot GRX access and the need for a reliable GTP reference source. Use of the contractor GTP reference environment is being explored.
- TDB-E have received an update briefing from project. TDB-C to follow.


## [edit] 7 December 2009

## Present:

- Working with OPS to restore GRX mobile traffic. This is currently our top priority. We are also working with GTE to make the GRX collection environment more robust.
- Working with TDB/NGE to schedule the IV\&V (I\&T) of NGE QFDs and Mobile Converged Events.
- Project headline milestones include:
- Rework of Converged Events and 10G GTP following pilot/derisk delivery.
- 7 Apps/Variants due for Experiment capability on 9 April.
- OPS are working to specify their App exploit requirements.
- BA and MTI are now more aware of Mobile requirements and the potential impact this has on their respective programmes, e.g. GOLDENEYE. Engagement continues.
- Business Changes to be finalised/agreed today. Benefits also being finalised by $\square$

[^0]
[^0]:    - The project's Wiki site has had a significant restruring, and is now robust enough to support higher usage. Project and engineering communications continue to migrate onto the wiki.
    - Two weeks to Christmas!
# [edit] 30 November 2009 

## Present:

- Business change for Thread 4 now crystallised.
- The report outligning the processes for engagement for new Mobile Apps into TPS now approved.
- Customer requirements need to be base lined.
- SIM Card exploitation - discussions progressing.
- Target Presence data (mostly C2C) needs to be added to the convergence strand ASAP. Currently looking at adding Presence capability to TERRAIN. There may have to be a trade-off against existing planned deliverables.
- Use Case 8 (Identify Target's Mobile Communications) needs volumetrics study.
- Need NGE planning delivery dates.
- Timescales for Contractor delivery of Mobile Apps / IPP processing capability need to be addressed/clarified.
- MAPL and PPL pages are being merged - the business strands stay separate.
- Use Case Realisations have all been updated. To explore MOOD's web publishing feature for productivity gains.
- New Use Case in hand for New Selector Types - this needs to be a sustainable business process.
- GCWiki suggested as a viable collaborative tool for multi-disciplinary collaborative pushes.

Retrieved from
Category: Mobile Applications Project

## Views

- Page
- Discussion
- Edit
- History
- Delete
- Move
- Watch
- Additional Statistics

Personal tools

## 1

- My talk
- My preferences
- My watchlist
- My contributions


## Navigation

- Main Page
- Help Pages
- Wikipedia Mirror
- Ask Me About...
- Random page
- Recent changes
- Report a Problem
- Contacts
- GCWeb


## Search

Go Search

## Toolbox

- What links here
- Related changes
- Upload file
- Special pages
- Printable version
- Permanent link

Powered by MediaWiki

- This page was last modified on 1 May 2012, at 11:44.
- This page has been accessed 64 times.
- 

All material is UK [http://www.gchq/organisation/ck/opensource/policy_strategy/copyright/ Crown Copyright] © 2008 or is held under licence from third parties. This information is exempt under the Freedom of Information Act 2000 (FOIA) and may be exempt under other UK information legislation. Refer any FOIA queries to GCHQ on
$\square$
$\square$

- Privacy policy
- About GCWiki
- Disclaimers

TOP SECRET STRAP1 COMINT
The maximum classification allowed on GCWiki is TOP SECRET STRAP1 COMINT. Click to report inappropriate content.
