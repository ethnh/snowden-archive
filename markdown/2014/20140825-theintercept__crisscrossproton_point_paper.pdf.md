# SUBJECT: CRISSCROSS/PROTON 

PURPOSE: Provide DIRNSA information on subject.

## BACKGROUND:

(U) History of CRISSCROSS/PROTON (how did it come about, when, and by whom.)

- (S//OC, NF) Project CRISSCROSS began in the early 1990's when CIA and DEA collaborated on a database and analytical tool suite to perform link analysis and cross-reference lookups against DEA and CIA collected telephone billing records and phone directories.
- (S//OC, NF) NSA Office of Crime and Narcotics requested the software and database capabilities of CRISSCROSS to enhance SIGINT data. CRISSCROSS proved extremely successful at identifying new phone numbers associated with 'lost' drug targets and locating additional targets of interest. Expanding the coverage from Latin America to worldwide then enhanced target development efforts across all NSA product lines.
(U) Current CRISSCROSS/PROTON Agreements.
- (S//OC, NF) All CRISSCROSS/PROTON Agreements are via bilateral Memoranda of Understanding (MOU) and exist between CIA, DEA, NSA, DIA, and FBI. DEA and FBI do not currently share data with each other.
- (S//OC, NF) DIA provides support to various DoD elements (e.g JICs/JACs and other Service Intelligence structures) as specified in MOU Addendums.
(U) How current data in CRISSCROSS/PROTON is "minimized" and by what standards.
- (S//OC, NF) From its inception, NSA has only provided telephony data to CROSSCROSS/PROTON, which constitutes: date, time, duration, called number and calling number. NSA "minimizes" this metadata prior to its transmission of data to CIA.
- (S//NF) NSA data is pulled from the FASCIA and HOMEBASE systems and transmitted to a NSA terminal in CIA's PROTON Project Office.
- (S//SI) For U.S. and $2^{\text {nd }}$ party numbers, minimization is achieved by replacing the rightmost 4 digits with four $x$ 's.
- (S/SI) The classification of the NSA call-event records is CONFIDENTIAL NOFORN.
- (S/OC, NF) NSA Office of General Counsel ruled that the data contributed by CIA, DIA, DEA, and FBI does not need to be minimized by NSA before being incorporated into the NSA PROTON system as each MOA signatory must "minimize" according to their own authorities.
(U) How CRISSCROSS/PROTON operates today (data flows/tape courier, tools, etc.)
- (S/NF) PROTON is a proprietary system architecturally inconsistent with DoD and NSA development guidelines and environment. It requires specific licensing and maintenance expenses and currently cannot be integrated with other tools.
- (S/OC, NF) Data is transferred from NSA, DIA, and FBI to CIA electronically or by courier delivery of magnetic tapes.
(U) Current proposals to modify (pending) CRISSCROSS/PROTON with the addition of other data elements/content/procedures
- (S/OC, NF) New communications technologies necessitated evolution of the CRISSCROSS software. The CRISSCROSS system only handled five call-record fields: date, time, duration, called number and calling number. PROTON goes further and analyzes additional data fields that are specific to cell and satellite phones, such as IMEIs and IMSIs, lat/long coordinates. PROTON also analyzes email headers (not content), SMS text messages, SIM cards, travel records (passport \#, flight \#, description), VISA application data and excerpts from CIA intelligence reports.
- (S/OC, NF) CIA, DIA, and FBI have added these additional data types to PROTON and share this data with NSA. However, NSA has never agreed to expand its contributions to PROTON.
- (S//OC, NF) PROTON performs entity analysis/contact chaining across data types. Users may search on a target entity's phone number and PROTON will return the associated email, cell phone, call records, street address, and CIA intelligence report escerpts.
- (S//OC, NF) PROTON tools find other entities that behave in a similar manner to a specific target, it also identifies correspondents in common with two or more targets, identifies potential new phone numbers when a target switches phones, and identifies networks of organizations based on communications within the group.
- (S//OC, NF) PROTON provides search capabilities for exploiting commercial phone books and data that do not conform to a particular type, such as escerpts from CIA intelligence reports.
(U) Current NSA contribution to CRISSCROSS/PROTON (data elements/number of records to date/records per week/month, etc.)
- (S//OC, NF) CIA, DIA, FBI, and DEA contributions over a three-month period totaled 11.7 billion records (which includes many records that are not "communications-metadata contact records".)
- (S//SI//NF) NSA contributions over the same three-month period totaled 4.2 billion records (again, only limited to telephony contact data). (Note: under the NSA proposal to create an IC-wide communications metadata repository, NSA's contribution would be in the 100's of billions of contact records- telephony and DNI contact records.)
(U) How NSA currently uses CRISSCROSS/PROTON in conjunction with other NSA metadata repositories and tools.
- (S//OC, NF) NSA analysts use Proton to perform analysis against data from CIA, NSA, DEA, FBI and DIA in a single common interface. Results provide additional targets of interest for all product lines. Merging the data produces a more complete picture of the target's communications and activity.
- (TS//SI//NF) NSA Users reported the following regarding the importance of PROTON:
- (S) SIGINT analysts in Iraq attributed PROTON for successes at locating and apprehending High Value Individuals (HVIs). PROTON had the information they needed to get U.S. troops in the right location.
- (S) PROTON was critical in capturing a HVI who was wanted by the FBI and AFOSI for terrorist related activity in Denver.
- (S//SI) PROTON provided the location information of a money eschange house that was connected to a Pakistani militant group.
![img-0.jpeg](img-0.jpeg)

- (S) PROTON allows a single stop to find registration information for phones that are not being used by the person to whom they are registered. This is particularly important for front companies, where tying multiple phones to the same registration can provide critical information."
(S) SID is recommending that a DNI IC-wide central communications metadata repository be established and reside at NSA and that DIRNSA/CHCSS be made Executive Agent for this IC repository. NSA and its foreign SIGINT partners stand alone in conducting metadata analysis on such a large scale and as a result, our tools and methodologies, as well as the infrastructure employed, are well tested and have been proven efficient and effective. We already extensively share metadata internally within the NSA/CSS enterprise and, having recently reached agreement with our Second Party partners, are ready to begin implementing that agreement to share Second Party metadata writ large.
(S//NF) Rather than continuing to push communications metadata out to the PROTON repository, we propose using the existing IC shared information space ICSIS (Intelligence Community System for Information Sharing) on INTELINK and have IC users come in through an existing tool to pull data from metadata repositories resident at NSA. We would implement IC access to our GLOBALREACH federated query service via accounts and access verified by PKI certificates. This service will provide the access requested and permit the auditing of such repository users. We believe we can have GLOBALREACH capability ready for the IC within approximately one to two months of a decision to proceed with this proposal.
(U//FOUO) ORIGINATORs: and
for the IC-metadata proposal, and
for CRISSCROSS/PROTON, 22 Feb 06
