![img-0.jpeg](img-0.jpeg)

# "The EDGE" 

National Information Assurance Research Laboratory (NIARL) Science, Technology, and Personnel Highlights

## September 2008 Edition

![img-1.jpeg](img-1.jpeg)

## (U) Message from the NIARL Director:

(U//FOUO) Welcome to the September 2008 edition of the National Information Assurance Research Laboratory (NIARL) newsletter. The NIARL is designated as the R2 organization within the NSA Research Directorate. NIARL/R2 is responsible for conducting and sponsoring research in technologies and techniques needed to secure America's future information systems. While breaking new ground is certainly rewarding, the overall goal for this research and exploration is to identify concepts and solutions to reduce the Information Assurance (IA) risks facing our nation's critical information systems.
(U//FOUO) Within R2's general IA research thrusts of Crypto-Math, IA Engineering, and Defensive Computing, there are specific "Focus Areas" dedicated to existing and/or anticipated critical challenges and technical IA risks. Focus Areas encompass topics such as Research Integration, High Confidence Software and Systems, Secure Wireless Multimedia, and Security Enhanced Operating Environments. For a complete listing of R2 Focus Areas please refer to the R2 website at
(U//FOUO) In this issue of The EDGE we examine the Research Integration Focus Area and the associated IA research challenges of bringing research concepts together, providing relevant mission context, and presenting IA approaches to customers and stakeholders. R223 leads the Research Integration Focus Area and is charged with shepherding IA concepts and innovations into the research prototype and demonstration stage. Please see the article "The Research Journey from Passion to Prototype" for a detailed discussion of this topic.
(U//FOUO) I am sincerely interested in your feedback and suggestions, and I ask that you email your comments to $\square$ R2 Office Manager, at $\square$ We look forward to hearing from you!

## [E]tical Work

Derived From: NSA/CSSM 1-52
Dated: 20070108
Declassify On: 20320108
TOP SECRET//COMINT//REL TO USA, AUS, CAN, GBR, NZL//20320108
(U) Contents
(U//FOUO) Information Sharing Roadmap Initiative
(U) Summer Mathematics, R21, and the Director's Summer Program
(U//FOUO) Support for 154 Code Review
(U//FOUO) Key Management Modeling Research
(U) The Research Journey from Passion to Prototype
(U) R222 Photonic Logic Program Review at Sandia National Laboratories
(U//FOUO) Sandia Trip Highlights R225's Anti-Tamper Research Progress
(U//FOUO) R225/Department of Energy Engagement Yields Idaho National Labs Research
(U//FOUO) CLARIFYMIND Wireless Pilot Technical Exchange with Canadian Representative
(U//FOUO) R22 Continues Collaboration with NSA CTO/TS via Secure Tokens Talk
(U) R23 Supports Graduate Math Program Large Graph Research
(U) OpenSolaris ${ }^{\left({ }^{(M}\right)}$ FMAC: Bringing the Flask Mandatory Access Control Architecture to OpenSolaris
(U//FOUO) R23 Contributes Behavioral Anomaly Detection to IDA/CCS DISTILLERY SCAMP
(U//FOUO) HAIRBALL Deploys GraphViz for POPEYESEAR: Visualization Techniques for Computer Network Defense
(U//FOUO) Personnel News
# (U) From the NIARL Technical Director's Desk: 

![img-2.jpeg](img-2.jpeg)
(U//FOUO) Information Sharing Roadmap Initiative
(U//FOUO) Recently, I was asked to lead a small team, with representation from across the Information Assurance Directorate (IAD), the NSA/CSS Commercial Solutions Center (NCSC), and the Research Directorate, to develop an IAD roadmap for information sharing. Obviously, this is not the first time an Agency or organization has developed a roadmap on this topic. For example, community roadmaps were developed by the Program Manager for Information Sharing Environment (PM-ISE) at the Office of the Director of National Intelligence (Information Sharing Environment Implementation Plan) and the Global Information Grid (GIG) Information Assurance Portfolio (GIAP) management office (System Technology Evolution Plan (STEP) for the Secure Information Exchange (SIE) thread of the GIG Information Assurance Architecture). Unlike previous community efforts, this activity is focused on developing an internal IAD information sharing roadmap.
(U//FOUO) So why is an internal IAD information sharing roadmap needed? While there are many reasons, the primary reasons are to provide a long term IAD vision for information sharing that is common across the corporation, to provide a shared context (e.g. a corporate description of information sharing and the necessary activities to achieve information sharing), and to provide a tool to synchronize and anticipate individual IAD, NCSC and Research activities related to information sharing. In a nutshell, this roadmap is intended to be a starting point for harmonizing all IAD activities related to information sharing over an extended timeframe (e.g. 5-7 years). Our goal is not to create a roadmap that competes with existing community roadmaps. Our approach will be to synthesize existing community roadmaps into an internal roadmap that drives IAD investments in information sharing. Lastly, our roadmap will be a living document and will be revised as the timeline moves to the right, or as IAD learns more about information sharing requirements.
(U//FOUO) POC: Technical Director/R2.

## (U) Crypto-Math Corner:

(U//FOUO) For general information on R21 Cryptograt hic IA Research's capabilities and current efforts, please visit the R2 web site. or the R21 homepage at link.
# (U) Summer Mathematics, R21, and the Director's Summer Program 

(U) The Director's Summer Program (DSP) is the agency's premier summer program for mathematics undergraduates. Since its inception in 1990, the mission of the DSP has not been simply recruitment, (though a small but steady percentage of DSP participants do come back to work at NSA, often after obtaining an advanced degree), but rather an outreach effort aimed at attracting the best mathematics students from around the country, educating them about mathematics at NSA, and thus establishing ties with the future leaders of the outside mathematics community.
(U//FOUO) While the DSP is hosted by the Mathematics Research Group, the technical directors come from across the Agency. In 2008 the technical directors were
(1) (R21), and (S31223). This year's 22 participants were culled from 260 applicants. Over 12 weeks, students worked in small teams with NSA mathematicians to develop real-world solutions to classified, operational problems.
(U//FOUO) Over the years, R21 personnel have supported the DSP both as project mentors, who propose a project and guide a small group of students (usually a 12-week, half-time commitment), and as technical directors of the program, who select and interview the students, find projects and mentors, and serve as general technical and administrative support full-time during the summer (usually a 2-year, half-time commitment).
(U//FOUO) This year, in addition to presenting their results to both the Director and Deputy Director of NSA, the DSP was invited to give classified presentations to a professional staffer on the Senate Select Committee on Intelligence (SSCI) as well as two members of the SSCI Technical Advisory Group.
(S//SI/REL) Projects from DSP 2008 of possible interest to R2 include: RANDOMIZERS, a study of open source randomizers, TUNDRA, research of a new statistic for codebook analysis, and CLOUD, implementing graph algorithms in a cloud computing environment. Short summaries follow.
(S//SI//REL) RANDOMIZERS -- Because of their use in the generation of keying material, randomizers play a critical role in modern cryptographic systems. The RANDOMIZERS project focused on two popular commercial software randomizers: Open SSL's randomizer and /dev/random. The DSP students researched the quality of these randomizers by measuring entropy and by considering cryptanalytic attacks (e.g., Forward Security). The students confirmed an outside attack on /dev/random, but they also showed that this attack is not as strong as the outside paper claimed. They found no obvious weaknesses in Open SSL's randomizer. Finally, the students examined a mixing component consisting of a shift register with a contribution from an entropy source (modeled as Bernoulli- $p$ bits). They determined a theoretical bound on the number of register steps needed to reach full entropy given $p$ and the polynomial driving the shift register. This project was supported by
of 1735 .
(TS//SI//REL) TUNDRA -- Electronic codebooks, such as the Advanced Encryption Standard, are both widely used and difficult to attack cryptanalytically. NSA has only a handful of in-house techniques. The TUNDRA project investigated a potentially new technique -- the Tau statistic -- to determine its usefulness in codebook analysis. This project was supported by of R21.
(S//SI//REL) CLOUD -- Cloud computing is a paradigm to perform massive computations in parallel on a cluster of computers via a "map-reduce" model. The DSP students researched how amenable cloud computing is to various graph algorithms. The team successfully implemented the graph algorithms $k$-cores and $k$-trusses as well as two Agency contact chaining algorithms, STARFIRE (developed by DSP 1999) and CARPAT, in the map-reduce framework. Their research suggests most graph algorithms fit naturally in the framework. Further, this framework supports the ability to process larger data sets. This project was supported by of R1.
(U//FOUO) This summer the students made good progress on these and five other projects. A report detailing all of the work done will be published by R1 in the fall of 2008.
(U//FOUO) POC: Dr. $\square$ R211,

# (U//FOUO) Support for I54 Code Review 

(U//FOUO) Earlier this year Chief of I54, solicited volunteers to support a DIRNSA and Director of IAD chartered review of approximately 100,000 lines of Ada 83 code. $\square$ forward deployed from R21 and serving as I542 Technical Director, enlisted R213 to provide support with automated software analysis tools.
(TS//REL R213, led the automated analysis effort using the tool PolySpace for Ada to analyze the code. PolySpace for Ada employs "abstract interpretation" to analyze code for a variety of errors such as uninitialized variables, integer overflow, et cetera. The initial automated analysis identified some non-standard software features requiring more extensive examination. $\square$ then teamed with R213, to assist with the analysis and provide results to $\square$ 1543. As noted by Mr. $\square$ the automated code analysis discoveries provided "valuable" results, and complemented a parallel 154 manual code analysis effort by highlighting several items undiscovered by the manual analysis team.
(TS//REL) Analyzing and debugging software code on fielded systems is a time-consuming, expensive operation. Using automated techniques to identify coding abnormalities and bugs in system software prior to fielding reduces the overall cost of fixing software errors by an order of magnitude and significantly increased the quality of the deployed software. To this end, R213 continues to research the development of software environments and software languages focused on integrating automated analysis within the design and development stages of the software development lifecycle.
(U//FOUO) POCs: $\square$ R213, (301 R213,
# (U//FOUO) Key Management Modeling Research 

(U//FOUO) R21 is approaching two significant milestones in Key Management Modeling (KMM) research. First, the researchers appear to have found a proof and analysis technology that is robust enough to do meaningful formal analysis of real key management systems. KMM is now making use of the Cryptographic Protocol Shapes Analyzer (CPSA) developed under contract to R213. CPSA was designed to analyze cryptographic protocols so KMM is now expressing key management systems as high-level protocols in order to apply CPSA. The KMM researchers have been working with Mitre, and changes to CPSA have already been made to enable it to be applied to KMM more directly.
(C//REL) Additionally, KMM is being used for the first time to model a real-world key management system. The United Kingdom (UK) is designing a new key management architecture as part of its Secure Management Infrastructure (SMI) effort. The initial UK architecture is simple enough to make it a good candidate for modeling while still allowing analysis to be accomplished on a real system. Furthermore, the UK has its own project to produce a formal specification of the key management architecture in Z, which will provide invaluable input to KMM. A draft model is currently under development, and if sufficient progress is achieved, R21 will be presenting the results at the 5-Eyes Key Management Strategy Group (KMSG) in Ottawa in October 2008.
(U//FOUO) POC: R212.

## (U) IA Engineering Exchange:

(U//FOUO) For general information on R22 IA Engineering Research's capabilities and current efforts, please visit the R2 web site www.iae.neuromedia.com/or use the R22 wiki link:

## (U) The Research Journey from Passion to Prototype

(U//FOUO) As noted in the NIARL Director's introduction, Research Integration (R223) is the NIARL Focus Area responsible for taking IA discoveries into the research prototype and demonstration stage. Along the way, the team explores and addresses critical assurance challenges facing our current information infrastructure, as well as those emerging against our future systems.
(U//FOUO) To explore the goals of Research Integration, let's follow some distinct research efforts from their origins toward the integrated prototype and demonstration stage. For this example, we'll use a well-understood assurance problem given our current operational
environment of multiple networks at various security levels - namely, the need for users to access multiple systems (also known as domains) in a secure way.
(U//FOUO) The central purpose of most research is to explore what's "next." Instead of a known desired end-state, this process often begins with a question, such as "are there better approaches to secure software?" - many ideas are then tested to try to find the answer. That particular question remains central to R213 High Confidence Software and Systems (HCSS) Focus Area research into how Formal Methods and mathematical proofs could ensure the "correctness" of software design. In this example, the HCSS team explored possible solutions and eventually developed a small-scale, Java-based proof-of-concept.
(U//FOUO) Meanwhile, in other areas of NIARL, another question was being asked within the Authentication team, "how can commercial smart card technologies be leveraged to provide assured identity for access to sensitive systems?" Over the years, smart cards (and smart card chipsets) rapidly progressed from their origins storing monetary value for European pay phones, to then becoming unique identifiers for mobile phones, and ultimately finding use as personal identification (and even DoD user authentication for unclassified systems). As the technology evolved, IA research explored approaches to leverage these technologies toward our goals. But that sparked other questions, such as "what do we do about software from unknown or risky sources?"
(U//FOUO) The "a-ha!" moment came from a convergence of these two problem sets courtesy of the Java Card standard for smart cards. Could Formal Methods lead to a proven Java-based operating system and provide assurance for commercially-based smart cards? In partnership with HCSS, Research Integration took the Formal Methods proof-of-concept approach and applied it to the real-world smart card problem. The lofty goal? Assured (and unclassified) multi-domain tokens for community identity and authentication.
(U//FOUO) The resulting Tokens Assurance Software research within Research Integration just completed the prototype of a functional and mathematically proven Java Card operating system. In addition, these software assurance techniques were expanded to develop tools to create assured applets to run on the cards. We will also soon complete some advanced hardware prototypes featuring physical protection concepts which will further demonstrate the "integrated" potential for how to provide strong authentication for access to critical systems.
(U//FOUO) To extend the concept, Research Integration will leverage additional NIARL exploration into yet another pressing IA research question, "how can virtualization technologies provide the foundation for future trusted computing platforms?" In partnership with fellow Focus Areas, Research Integration is prototyping early versions of these approaches to investigate how they could enable assured information sharing, authentication and access control, as well as mobility for users. In this way, the initial breakthroughs of software assurance, secure tokens, and platform trust could start to create answers to real operational questions, such as "How can we transform the way user identity is protected to enable cross-community collaboration?"
(U//FOUO) So while "passion" for IA discovery is not unique to Research Integration, our objective is to put these advanced technologies into a form that highlights their potential to address significant assurance questions. No matter the origin, the potential technology solutions that emerge from IA research are designed for significant breakthrough. However, a particular innovation, in and of itself, provides limited benefit unless it can advance the science, solve a problem, and ultimately reach customers. The aim of the R223 Research Integration team is to reach those customers and showcase the potential for NIARL research to become a decisive advantage against network adversaries. Please contact us if you would like to learn more about our research efforts and see our latest creations.
(U//FOUO) POC: | Chief R223,|

# (U) R222 Photonic Logic Program Review at Sandia National Laboratories 

(U//FOUO) From 19-21 August 2008| | and |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | 
# (U//FOUO) POC: 

## (U//FOUO) Sandia Trip Highlights R225's Anti-Tamper Research Progress

(S//REL) Use of commercial components in a high assurance solution for national security applications will require physical protection mechanisms. In the past, with government built solutions, anti-tamper was part of the design and manufacture process. Today, use of COTS will require the government to apply these protections after production. R225's Intelligent Reaction Anti-Tamper (AT) research program showcased the ability to provide these physical protection mechanisms at a recent program review at Sandia National Laboratories.
(S//REL) Several key technologies were demonstrated:

- Multi-layer conformal AT on printed circuit boards with integrated control logic;
- iPhones with hard aftermarket device encapsulation; and
- Chip packages retrofitted with active anti-tamper capability, including internal power.
(S//REL) Remaining FY08 research into conformal AT technology will support R223's secure token effort. Starting in FY09, I823 will assume full responsibility for further development of this AT technology as a part of R225's partnerships forged to realize a full life cycle: from research through implementation. R225 and I823 are working together to advance the aftermarket device encapsulation technology to the same level of technical readiness, with SID's NUCLEARWINTER team as a potential initial customer. R225 will continue research on the modified chip packaging technology in FY09, and will work with IAD to identify potential end-users.
(U//FOUO) POC: $\square$ and $\square$ R225, $\square$


## (U//FOUO) R225/Department of Energy Engagement Yields Idaho National Labs Research

(S//REL) Researchers from Idaho National Labs (INL) visited NSA on 26 August 2008 to demonstrate INL progress on research into secure erasure for commercial memory modules. INL is moving towards a method of retrofit zeroization capability for synchronous dynamic random access memory (SDRAM) in commercial desktops, with an initial prototype expected by the end of FY08. This work is similar to R225's Adaptive Zeroization research, but trades greatly reduced applicability and scope for lower risk. Personnel from R225, IAD's Microelectronics Anti-Tamper Solutions Branch (I8231), and IAD's Cryptographic Engines, Modules, and Tokens Division (I853) participated in the discussion. This research was sponsored by R225, and funded by the Department of Energy's 2008 Applied Technologies Program. R225 is beginning discussions with its IAD partners to determine the best way to move forward with integrating INL's work into NSA's future anti-tamper mission.
(U//FOUO) POC: $\square$ R225
# (U//FOUO) CLARIFYMIND Wireless Pilot Technical Exchange with Canadian Representative 

(U//FOUO) $\square$ and $\square$ of the R224 CLARIFYMIND Wireless Pilot Team met with of Canadian Security Establishment Canada (CSEC) who is currently assigned to the Canadian Liaison Office at NSA. The meeting was a follow up to $\square$ May 2008 CLARIFYMIND presentation to the 5 Eyes Information Assurance Research Conference at NSA. $\square$ described the new CSEC building under construction, the need for wireless communications in the facility, and the CSEC efforts underway to consider various wireless solutions. The R224 team briefed $\square$ on the CLARIFYMIND wireless pilot, current research efforts, and planned future activities $\square$ was very interested in considering CLARIFYMIND as a potential pilot application. He plans to share the CLARIFYMIND potential pilot partner information with CSEC decision-makers and then schedule a follow-up technical exchange with the R224 Team.
(U//FOUO) POC: $\square$ R224.

## (U//FOUO) R22 Continues Collaboration with NSA CTO/TS via Secure Tokens Talk

(U//FOUO) The Information Assurance Engineering Research Office (R22) is continuing a collaboration initiative with the NSA/CTO Chief Information Security Officer (CISO) and Chief Information Officer (CIO) Staff (TS) through an exchange of ideas via TS-sponsored technical talks. R22's objective is to assist TS with improving the security of critical IT systems as well as obtaining feedback and information on emerging hard problems to consider for future research. In addition, the regular exchange with TS helps connect R22 researchers to a potential new base of customers and partners.
(U//FOUO) $\square$ the R223 lead researcher for secure tokens discovery, presented on 8 August 2008 at the TS Technical Talk Forum. His discussion centered on the Tokens Research Roadmap, the current status of development efforts underway through partnerships with IAD, and current utilization of interim capabilities on CES laptops. TS personnel and other Agency representatives who deal with tokens/smartcards responded positively and launched a dialogue on many issues that encompassed operations, policy, technical transfer, and productization challenges. While there were different implementation issues raised for a variety of customer sets, the common end vision is an assured identity token in a smartcard format. The R223 token research program is in line with this vision and all capabilities will be compatible and can be transferred onto a smartcard format. Both DOD and IC customer needs are addressed as a part of the R223-led research strategy.
(U//FOUO) POC: $\square$ R224
# (U) Defense Computing Bytes: 

(U//FOUO) For general information on R23 Defense Computing Research Office's capabilities and current efforts, please visit the R2 web site. We use the R23 homepage.

## (U) R23 Supports Graduate Math Program Large Graph Research

(U//FOUO) For 12 weeks over the summer of 2008 the Graduate Math Program (GMP) ${ }^{1}$ participants wrestled, wrangled, quantified and processed more than 200GB of network traffic metadata generated by R23's FLOWBEE project. FLOWBEE is a spin-off of the POPQUIZ project, which collects network metadata on high bandwidth protocols such as HTTP, SMTP, and DNS. FLOWBEE uses novel techniques to efficiently recognize and discard duplicate relations, significantly reducing the volume of saved data. This data reduction, in combination with the highly efficient POPQUIZ ${ }^{2}$ processing framework, allows FLOWBEE to collect metadata for every session on high-speed links.
(U//FOUO) This rich and varied dataset provided fertile ground for their explorations in large graph analysis and characterization. Led by Technical Directors from R1 and R6, participants focused on finding malicious activity in the data, modeling graphs produced by the FLOWBEE data, and investigating high-performance computing architectures to determine their applicability to processing FLOWBEE data and related large graph problems.
(U//FOUO) As the problem supporters for GMP, R23's DIO team provided data, loaded and indexed the data in a MySQL database, and installed the FLOWBEE Surf web interface in the GMP's lab. R23 also provided training and consulting on the FLOWBEE data and associated processing tools, presented findings from prior research, and participated in workshop and brainstorming sessions during the course of the summer. On 31 July 2008, the GMP and R2 DIO team members presented their findings to DIRNSA and D/DIRNSA.
(U//FOUO) This summer's GMP work resulted in numerous improved capabilities that have been incorporated into existing R23 technology. The big wins from this activity were:

- A new algorithm for detecting web spam, which found confirmed new malicious hosts
- An improved BadRank algorithm for rating the badness of a host based on its connections

[^0]
[^0]:    ${ }^{1}$ (U//FOUO) GMP is a competitive 12-week summer program run by R1. It provides an opportunity for exceptional mathematics graduate students to work directly with NSA mathematicians on mission-critical problems and experience the excitement of the NSA mathematics community.
    ${ }^{2}$ (U//FOUO) See July 2008 EDGE Newsletter for additional information on POPQUIZ.
- An improved random forest classifier to detect malicious hosts, which found confirmed new malicious hosts
- An implementation of BadRank for the Cray XMT
- A Hadoop MapReduce implementation of PageRank
- New insights into the strengths, weaknesses, and scalability of the KronFit graph generation algorithm, including new proofs of several properties
(U//FOUO) POC: $\square$ R23, $\square$

(U) OpenSolaris ${ }^{\left({ }^{(M}\right)}$ FMAC: Bringing the Flask Mandatory Access Controls Architecture to OpenSolaris
(U) Flexible Mandatory Access Control (FMAC) for OpenSolaris ${ }^{\left({ }^{(M}\right)}$ is a joint NSA and Sun Microsystems Inc. project to add the Flask architecture to the OpenSolaris operating system. The Flask architecture provides flexible support for a wide range of security policies, enabling integration of different policy engines and the configuration of the security policy to meet the specific security goals for a variety of computing environments. The flexible mandatory access controls supported by the Flask architecture enable the confinement of flawed and malicious applications and the enforcement of confidentiality, integrity, least privilege, and assured invocation goals. The Flask architecture has been successfully applied to several other operating systems via the SELinux, SEBSD, and SEDarwin projects as well as to other software components such as hypervisors (Xen), windowing systems (X), and database systems (PostgreSQL).
(U) The initial FMAC code base was contributed by the NSA to OpenSolaris based on a version of the Flask code that predated any involvement by the Linux community. This code was then integrated into the OpenSolaris code and adapted by $\square$ a Sun engineer who is the co-lead of the FMAC project. This code was first released publicly on the FMAC project web site in May 2008. When built, it produced a policy compiler and a kernel capable of loading the resulting policy into the security server.
(U) Since that first release, joint development by the NSA and by Sun Microsystems has proceeded rapidly. Support for new system calls was introduced in June 2008, and support for labeling processes was introduced in July 2008. Several utilities have been created for controlling and interacting with the system. Current design and implementation discussions are focusing on how to best support file security labeling in OpenSolaris, particularly for the ZFS filesystem. Once file labeling is supported, the next steps will include support for domain transitions and permission checks on process and file operations. This will provide a base capability that can be used both to demonstrate the benefits of Flask and to further develop the remaining support for object labeling and mandatory controls.
(U//FOUO) POC: $\square$
# (U//FOUO) R23 Contributes Behavioral Anomaly Detection to IDA/CCS DISTILLERY SCAMP 

(TS//SI//REL) The 2008 Summer Conference on Applied Mathematical Problems (SCAMP) was hosted this summer in Bowie, MD at the IDA/CCS. This SCAMP focused on a specific category of attacks and intrusions targeted against U.S. critical national infrastructure. Commonly known in the DoD community as the BYZANTINE HADES (BH) attacks, these intrusions are believed to originate from the People's Republic of China. The main goals of the SCAMP were to define and implement novel behavioral-based techniques that could better detect and respond to the wide array of BH attacks. R23's POPQUIZ framework provided the analytical applications to identify behavioral anomalies while DISTILLERY provided the stream-based platform from which to execute these applications.
(U//FOUO) A key factor to the success of the SCAMP was the availability of the SPADE programming language. Developed by IBM, SPADE enables the rapid development and prototyping of distributed stream-processing applications. Utilizing this language requires little programming expertise, as applications are described using high-level stream-centric constructs. A compiler handles the conversion of this description into native DISTILLERY application. The SCAMP participants, the majority having had little experience developing DISTILLERY applications, were able to quickly compose unique and complex applications. By not having to expend time learning a new low-level API, participants were able to focus their efforts on defining and implementing new detection techniques and methodologies.
(U//FOUO) POC. R23.

## (U/FOUO) HAIRBALL Deploys GraphViz for POPEYESEAR: Visualization Techniques for Computer Network Defense

(U//FOUO) On 12 August 2008 the R23 HAIRBALL project deployed its GraphViz v1.0 visualization tool to the NTOC floor as an addition to the POPEYESEAR interface. Following the deployment of TreeViz in Nov 2007, GraphViz is the second visualization tool deployed for operational use. The achievement reflects the ongoing research investment in new visualization techniques uniquely designed to support exploration and analysis of Computer Network Defense (CND) data.
(U//FOUO) GraphViz displays relationships from POPEYESEAR data as an interactive graph with dynamic, analyst-directed navigation. The dynamic navigation empowers analysts to locate subsets of the large POPEYESEAR database that are most relevant to their analysis. The graph-based display enables analysts to more easily perceive the connections existing in the data.
(U//FOUO) GraphViz has been built with an eye towards usability and rapid response. The interface provides Google-like search syntax and intuitive point-and-click control. Under the hood, the use of data preprocessing and indexing enables GraphViz to return results with
minimal wait time for the analyst. GraphViz is a Java application and uses Renoir as its graphing engine. As an added component of the POPEYESEAR interface, GraphViz is accessible to all NTOC operational analysts via the GROUPDIVE/BLUESASH network.

# (U//FOUO) POC: 

## (U//FOUO) Personnel News

## (U//FOUO) Visiting Researchers in R21:

- (U//FOUO) Recent arrivals in R21 include $\square$ of the Cryptologic Mathematician Program, who will be conducting research in Elliptic Curves, and $\square$ of the Applied Mathematics Program, who will be conducting research in Quantum Computing. In addition, $\square$ Iopielec of the Cryptanalysis Development Program will be arriving soon to begin conducting research in Cryptographic Hash Functions.
- (U//FOUO) At any given time, R21 typically hosts between 5 and 10 visiting researchers, mostly participants in the various math development programs at the Agency. These 6 to 9 month tours are a staple of the development program experience, and are coordinated through the R21 "intern czar" $\square$ Persons interested in learning more about tour opportunities in R21 should contact directly to get an overview of the office and to learn about currently available projects. (POC: $\square$ R213, $\square$


## (U//FOUO) Hail to R22 Newcomers:

- (U//FOUO $\square$ SNIP (System and Network Interdisciplinary Program) of 2011, will join R224: Secure Wireless Multimedia Focus Area, for a tour, starting Sept 15. Justin will be working on CLARIFYMIND-TS, specifically looking at available entropy sources, plus how to gather and provide them to the Random Number Generator within the CM-TS architecture. R21's draft paper entitled $\boldsymbol{A}$ Preliminary Architecture for a Software Randomizer for CM-TS will provide the basis for work. (POC: $\square$


## - (U//FOUO) recently joined R222 as a Lead Researcher after completing a PCS at GCHQ. A mathematician from the CMP class of 2000, $\square$ brings a wide variety of relevant hardware and software experience across a range of projects, encompassing Field Programmable Gate Array (FPGA) design, error correcting codes, high speed synchronization techniques and protocols to name a few. Throughout his career, $\square$ has won high regard as a leader and a mentor. $\square$ is a member of the High Speed Electronics team, where his initial focus will be on emerging technologies. (POC: $\square$
- (U//FOUO) an IDA/CCS Contractor and both SNIP interns will be joining the DIO team, beginning 2 September 2008. will be focused on developing new characterizations and methods for POPQUIZ. Both were recently part of the DISTILLERY SCAMP and plan on a 6 to 9 month tour to learn and to contribute to the DIO mission. (POC: $\square$ (00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
