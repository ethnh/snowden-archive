# CSEC SIGINT Cyber Discovery: Summary of the current effort 

Communications Security Establishment Canada
Covert Network Threats
Cyber-Counterintelligence

## Discovery Conference <br> GCHQ - November 2010
# Outline 

- CSEC SIGINT Cyber
- KOG (CCNE)
- GA4 (GND)
- CNT1 (CCI)
- CSEC SIGINT Cyber - Operational Discovery
- Network Based Anomaly Detection
- Host Based Anomaly Detection
- Contacts
# CSEC Cyber Counterintelligence 

![img-0.jpeg](img-0.jpeg)
# Counter CNE (KOG) 

- Part of CSEC CNE operations (KO)
- Recently formed matrix team
- Analysts and operators from CNE Operations, CyberCounterintelligence and Global Network Detection
- Mandate:
- Provide situational awareness to CNE operators
- Discover unknown actors on existing CNE targets
- Detect known actors on covert infrastructure
- Pursue known actors through CNE
- Review OPSEC of CNE operations
# Global Network Detection (GND) 

- Develop capabilities to improve the ability of the SIGINT collection system to detect Computer Network Exploitation and Computer Network Attack
![img-1.jpeg](img-1.jpeg)
- Help enable CSEC's CNE program through timely identification of vulnerable computer systems and foreign CNE methodologies/activities
- Act as technical liaison between IT Security and SIGINT for CNO issues
# Cyber Counterintelligence (CNT1) 

- Covert Network Threats (New Directorate within CSEC)
- CNT1 (Cyber Counterintelligence)
- CNT2 (Traditional Counterintelligence)
- CNT1 Mission
- To produce intelligence on the capabilities, intentions and activities of Hostile Intelligence Services to support Counterintelligence activities at home and abroad.
- Fusion of Cyber Analytic Skills with Traditional Counterintelligence Analytic Skills
- All Cyber-Counterintelligence Investigations should lead to Traditional Counterintelligence investigations.
# CSEC SIGINT CCI Discovery 

![img-2.jpeg](img-2.jpeg)
# CSEC CNE (K) - WARRIORPRIDE 

- WARRIORPRIDE (WP):
- Scalable, Flexible, Portable CNE platform
- Unified framework within CSEC and across the 5 eyes
- WARRIORPRIDE@CSE/etc. == DAREDEVIL@GCHQ
- xml command output to operators
- Several plugins used for machine recon / OPSEC assessment Several WP plugins are useful for CCNE:
- Slipstream : machine reconnaissance
- ImplantDetector : implant detection
- RootkitDetector : rootkit detection
- Chordflier/U_ftp : file identification / retrieval
- NameDropper : DNS
- WormWood : network sniffing and characterization
# KOG - ReplicantFarm 

- Created to leverage the WP XML output in a meaningful way
- Module based parser/alert system running on real-time CNE operational data
- Custom/module based analysis:
- Actors
- Implant technology
- Host based signatures
- Network based signatures
# REPLICANTFARM generic modules 

- Cloaked
- Recycler
- Rar password
- Tmp executable
- Packed
- Peb modification
- Privileges
- MS pretender
- System32 "variables" Other ideas....
- Strange DLL extensions
- Kernel cloaking
- Schedule at
- Ntuninstall execution
- hidden
# Generic modules : example 

my @runningProcs = xml_isProcessRunning( \$xml, 'svchost.\{1,3\\\.exe', 'winlogon.\{1,3\\\.exe', 'services.\{1,3\\\.exe', 'lsass.\{1,3\\\.exe', 'spoolsv.\{1,3\\\.exe', 'autochk.\{1,3\\\.exe', 'logon.\{1,3\\\.scr', 'rundll32.\{1,3\\\.exe', 'chkdsk.\{1,3\\\.exe', 'chkntfs.\{1,3\\\.exe', 'logonui.\{1,3\\\.exe', 'ntoskrnl.\{1,3\\\.exe', 'ntvdm.\{1,3\\\.exe', 'rdpclip.\{1,3\\\.exe', 'taskmgr.\{1,3\\\.exe', 'userinit.\{1,3\\\.exe', 'wscntfy.\{1,3\\\.exe', 'tcpmon.\{1,3\\\.dil' );
foreach my \$runningProc (@runningProcs)
\{
\$alertText . = "Suspicious process detected, legitimate exe named appended with string: " .
\$runningProc . ".\n";
Safeguarding Canada's security through information superiority
Préserver la sécurité du Canada par la supériorité de l'information
![img-3.jpeg](img-3.jpeg)

# CCNE/Opsec WPID Alerts 

## REPLICANTFARM

Note that the search is done with the fields as part regular expressions...
![img-4.jpeg](img-4.jpeg)

| WPID: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200: <br> 1200:
# EONBLUE 

- CSEC cyber threat detection platform
- Over 8 years of development effort
- Scales to backbone internet speeds
- Over 200 sensors deployed across the globe
![img-5.jpeg](img-5.jpeg)
![img-6.jpeg](img-6.jpeg)

Safeguarding Canada's security through information superiority
Cand
# Anomaly Detection Tools 

- There are currently over 50 modules in Slipstream
- RFC Validation
- Heuristic Checks
- Periodicity
- Simple Encryption
- Streaming Attack Detection
- Analyst Utilities
- Not all of these tools are 'YES/NO', some will require some work.
# Heuristic Example 

## - QUANTUM

- It's no lie, quantum is cool.
- But its easy to find
- Analyze first content carrying packet
- Check for sequence number duplication, but different data size
- If content differs within the first $10 \%$ of the pkt payload, alert.
# What's Next? 

- Anomaly Discovery at scale
- Multi-10G anomaly detection
- Cross Agency communication of anomalies
- Sometimes signatures aren't enough
- DONUTS!
- Everyone likes them:
- 5-eyes accessible DONUTS
- Discovery of New Unidentified Threats
- CSEC / GCHQ right now
![img-7.jpeg](img-7.jpeg)
# CNT1 - Analysis 

- Triage leads from KOG and GA4
- Links to existing intrusion sets?
- Pursue interesting leads
- Passive SIGINT collection
- Technical analysis
- Produce reporting
- Attribute
# Analytic Approach 

1. Begin with lead
2. Apply to SIGINT
3. Apply to CCNE
4. Track, research and report
5. Generate persona lead
6. Coordinate with traditional Cl
![img-8.jpeg](img-8.jpeg)
# Cyber-Specifics of the Analytic Approach 

## Network Traffic Analysis

- We have access to Special Source, Warranted and $2^{\text {nd }}$ Party collection in raw, unprocessed form
- Work very closely with protocol and crypt analysts


## Malware Analysis and Reverse Engineering

- Samples are received through passive collection and human sources


## Forensic Analysis

- Assist traditional Cl investigations and others
# CSEC Contacts 

![img-9.jpeg](img-9.jpeg)
