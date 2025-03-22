# Pay attention to that man behind the curtain: Discovering aliens on CNE infrastructure 

![img-0.jpeg](img-0.jpeg)

## CSEC Counter-CNE

Target Analytics thread SIGDEV Conference NSA - June 2010
# The need for Counter-CNE... 

- Foreign and friendly actors often encountered
- CNE operators do not pursue them beyond their targets
- Reporting groups need to be made aware
- OPSEC evaluation is needed
- Active pursuit of CNE actors: a different ballgame
# Outline 

- Introduction CCNE at CSEC
- CCNE tools and methods
- SNOWGLOBE
- De-confliction
# CCNE Group at CSEC 

- Part of CSEC CNE operations (K0)
- Recently formed matrix team
- Analysts and operators from CNE Operations, IO Reporting Lines and Global Network Detection
- Mandate:
- Provide situational awareness to CNE operators
- Discover unknown actors on existing CNE targets
- Detect known actors on covert infrastructure
- Pursue known actors through CNE
- Review OPSEC of CNE operations
# CCNE team 

![img-1.jpeg](img-1.jpeg)

Safeguarding Canada's security through information superiority
5
# CNE Toolkit: WARRIORPRIDE 

- WARRIORPRIDE (WP):
- Scalable, Flexible, Portable CNE platform
- Unified framework within CSEC and across the 5 eyes
- Do more with less effort
- Common framework for sharing code/plugins across the 5 eyes
- WARRIORPRIDE is an implementation of the "WZOWSKI" 5-eyes API
- WARRIORPRIDE@CSE/etc. == DAREDEVIL@GCHQ
- WARRIORPRIDE
- xml command output to operators
- Several plugins used for machine recon / OPSEC assessment
# WARRIORPRIDE 

![img-2.jpeg](img-2.jpeg)

Safeguarding Canada's security through information superiority
![img-3.jpeg](img-3.jpeg)
# WARRIORPRIDE plug-ins and output 

- Several WP plugins are useful for CCNE:
- Slipstream : machine reconnaissance
- ImplantDetector : implant detection
- RootkitDetector : rootkit detection
- Chordflier/U_ftp : file identification / retrieval
- NameDropper : DNS
- WormWood : network sniffing and characterization
- Already used for CNE OPSEC
- Used for precise identification and heuristics
# WP xml output (raw) 

```
<?xml version="1.0" encoding="UTF-8"?>
<response xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:noNamespaceSchemaLocation="U_FileCollectorLp/U_FileCollectorLp_2.15.xsd"><implant|
    d>51.1.2.160</implantId><transaction><transactionSource>50.0.0.101</transactionSource><tr
    ansactionId>320453</transactionId></transaction><timestamp><TLT>2010-02-
    23T15:53:06.366</TLT><UTC>2010-02-
    23T15:47:43.448</UTC></timestamp><errors><errorPlugin>0</errorPlugin><errorOs>0</error
Os></errors><commandInfo>fcstart</commandInfo><responseDetails></cstart><status>Succe
ss</status><standbyMode>FALSE</standbyMode></fcstart></responseDetails></response>
```
# WP SLIPSTREAM output (parsed) 

[2010/05/18 - 16:28:05 (UTC)] Transaction Id: 582966
U_SLIPSTREAM - <ssservices>
ImpiantId: <51.8.1.13>
Timestamp (UTC): 2010/02/09 06:42:42
![img-4.jpeg](img-4.jpeg)
# WP SLIPSTREAM output... drivers 

[2010/05/18 - 18:28:06 (UTC)] Transaction Id: 582968
U_SLIPSTREAM - <ssdrivers>
Impiantid: <51.8.1.13>
Timestamp (UTC): 2010/02/09 06:42:43
![img-5.jpeg](img-5.jpeg)
# REPLICANTFARM 

- Extend WP output to a signature based system: REPLICANTFARM
- Module based parser/alert system running on real-time CNE operational data
- Custom/module based analysis:
- Actors
- Implant technology
- Host based signatures
- Network based signatures
# CCNE/Opsec WPID Alerts 

File Edit View History Bookmarks Tools Help
![img-6.jpeg](img-6.jpeg)

## CCNE/Opsec WPID Alerts

## REPLICANTFARM

Note that the search is done with the fields as perl regular expressions...

## Example:

![img-7.jpeg](img-7.jpeg)

## Summary

## ALERIS

| WPID | Module: <br> mod_103_MM_DOGEOUSE.pl | Date: <br> 2010-01-21T15:36:35:96R | Tag: <br> MM | File name...datastorcircitive/201001/21/15 <br> CXID0000272485_18_V2010M01D21_H15M28859_MX642MU500NS0_RXID050_000_0 |
| :--: | :--: | :--: | :--: | :--: |
| Details: <br> Possible MM DOGEOUSE driver file: CWINNT\SNtUninstallQ2445988. <br> Possible MM DOGEOUSE driver file: CWINNT\SNtUninstallQ2445989夺fft sys <br> Possible MM DOGEOUSE driver file: CWINNT\SNtUninstallQ2445989埥rep.sys. <br> Possible MM DOGEOUSE driver file: CWINNT\SNtUninstallQ2445989/muffix inf |  |  | mod_24_reported/oparents.pl mod_11_prc/veps.pl mod_500_0D_MD01919.pl mod_01_polstersthorism.pl mod_21_subadults.pl mod_22_monars/drams.pl mod_22_hidom.pl |  |
![img-8.jpeg](img-8.jpeg)
# REPLICANTFARM generic modules 

- Cloaked
- Recycler
- Rar password
- Tmp executable
- Packed
- Peb modification
- Privileges
- MS pretender
- System32 "variables"
- Strange DLL extensions
- Kernel cloaking
- Schedule at
- Ntuninstall execution
- hidden


## Other ideas...
# Generic modules : example 

my @runningProcs = xml isProcessRunning( \$xml, 'svchost.\{1,3\\\.exe', 'winlogon.\{1,3\\\.exe',
'services.\{1,3\\\.exe',
'Isass.\{1,3\\\.exe',
'spoolsv.\{1,3\\\.exe',
'autochk.\{1,3\\\.exe',
'logon.\{1,3\\\.scr',
'rundll32.\{1,3\\\.exe',
'chkdsk.\{1,3\\\.exe',
'chkntfs.\{1,3\\\.exe',
'logonui.\{1,3\\\.exe',
'intoskrnl.\{1,3\\\.exe',
'ntvdm.\{1,3\\\.exe',
'rdpclip.\{1,3\\\.exe',
'taskmgr.\{1,3\\\.exe',
'userinit.\{1,3\\\.exe',
'wscntfy.\{1,3\\\.exe',
'tcpmon.\{1,3\\\.dil' );
foreach my \$runningProc (@runningProcs)
\{
\$alertText . = "Suspicious process detected, legitimate exe named appended with string: " . \$runningProc . ".\n";
\}
# RF specific signatures 

- KNOWN actor filenames, processes, covert stores:
- MAKERSMARK / FANNER
- SEEDSPHERE / BYZANTINE
- ALOOFNESS
- SNOWGLOBE
- VOYEUR
- SUPERDRAKE
- GOSSIPGIRL
- Infrastructure
- Known IP addresses
- Known DNS queries
- Other tools
# Specific signatures : example 

\# Check a known drivers present
my @driversPresent = xml isDriverPresent( \$xml, 'usbdev\l.sys', 'acpimem32\l.sys', 'usblink32ill.exe', 'll\$NtUninstallQ722833ll\$');
foreach my \$driver (@driversPresent)
\{
\$alertText .= "Possible MM CARBON driver detected: " . \$driver . ".\n";
\}
# Operations 

- Routine operations for CCNE investigations on current targets
- Execution of OPSEC related plugins
- Collection of files
- Examination of network activity
- Blanket approvals for addition of selectors to level 4 OPs against known actors: example WATERMARK operations against MAKERSMARK
- Standard operating procedures for level 2 - level 4 operataions against foreign CCNE actor infrastructures
# CCNE / OPSEC page on 5-Eyes K1SVN Wiki 

" Contains reverse engineering reports for CNE / IO consumption

- Even logs and notes for several actors
# CCNE operations - Covert Infrastructure 

- Some fusion of the WP and CCNE infrastructures
- Dedicated ORB for CCNE
- Unattributed dialups to the ORB
- Philosophy: use low hanging fruits against the actors (public exploits and tools if available)
- Discussions regarding repurpose of foreign toolkits
- De-confliction
# SNOWGLOBE 

- Provide the historical account of the activity on DOURMAGNUM (Imam Hussein University)
- Implant identified while investigating another unattributed actor
- rar archiving of emails on target
- Beaconing using HTTP to php-based listening post
# 2) CCNE/Opsec WPID Alerts - Mozilla Firefox 

File: Edit View History Bookmarks Tools Help

## 1) $\times$ ( 1

Most Visited Getting Started . Latest Headlines $\rightarrow$ LTT + Operations $<$ TVL $\rightarrow$ Opsec - k1svn - Trac $\square$ CCNE/Opsec Systems $\square$ http://cbells/system/info/
4) http://cbells/ $\qquad$ CCNE/Opsec WPID Alerts $\times$ $\square$ CCNE/Opsec WPID Alerts $\times$ Opsec - k1svn $\times$ Opsec - k1svn

## CCNE/Opsec WPID Alerts

Note that the search is done with the fields as perl regular expressions.
![img-9.jpeg](img-9.jpeg)

## Bideris Group:

## ALERTS

| WPID | Module: cnsd_700_SG_CNDCOPDP pl | Date: 2009-09-30T10:18:41:906 | Tag: SG | File name: <br> datac1nv:avs1nv:2009:09:30'10'TXDD000004573_18_Y2009S090355_H10M1 |
| :--: | :--: | :--: | :--: | :--: |
| Details: <br> Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcSnglcd -mld temp 168.rar c:MDAEMON'Users'Bu:a Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcSnglcd -mld temp 168.rar c:MDAEMON'Users'Bu:a Possible SNOWGLOBE CHOCOPOP process detected "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-500rar.exe" a -r -lnd -hplockless -apcNanarian -mld C:WDODOWS:TEMP-166.rar c:MDAEMON'Us:a Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld C:WDODOWS:TEMP-166.rar c:MDAEMON'Us:a Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-500 rar.exe" a -r -lnd -hplockless -apcNanarian -mld C:WDODOWS:TEMP-166.rar c:MDAEMON'Us:e Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu: Possible SNOWGLOBE CHOCOPOP process detected cnd.exe /C "c:RECYCLER:S-1-5-21-101796669-4102346875-220983236-50?rar.exe" a -r -lnd -hplockless -apcNanarian -mld temp 166.rar c:MDAEMON'Users'Bu:
# SNOWGLOBE on target 

## Possible SNOWGLOBE CHOCOPOP process detected:

cmd.exe /C ""c:\RECYCLER\S-1-5-21-101796669-4102346875-220983236-500\rar.exe" a -r -inul -hplockless -aprfeghhi -tn1d temp\168.rar c:\MDAEMON\Users\ihu.ac.ir\rfeghhi\md5*.msg">nul.
# SNOWGLOBE implant 

- Injects itself in svchost.exe
- No cloaking / no hooking
- Bootstraps in service called MSDTC64 (distributed transaction coordinator 64b
- Service entry is permanent
- Executable kept on disk in system32
- Crypto: 16 byte string XOR
- http beacons and tasking
- Actor observed upgrading on target
# SNOWGLOBE activity and attribution 

- Targeting is scarce but resembles CT / CP priorities
- French localisation seen in exploit PDFs (GCHQ)
- French commentary in the binary
- French binary name / developer path
- Observed in Iran, Norway, Greece, Belgium, Algeria, France, US targets
- Listening posts worldwide - several French legit sites
- Now seen in passive collection, several reports
# De-confliction : on CCNE operations 

- State-sponsored landscape is very busy
- CCNE Targets are de-conflicted
- Actors on CCNE targets are not
- Covert nature of foreign (and friendly actors) make deconfliction challenging
- Often need to refer to precise technology for identification
- CNE / CCNE from SIGINT + HUMINT need to get together on this issue
# De-confliction FAIL 

## - Actor discovered

- 5 eyes effort
- Several cohabitations
- At CSEC: 400 man-hours:
- Over 20 CNE Operations
- Passive Collection
- 4 Reports
- Reverse engineering
- Planning of active operations
![img-10.jpeg](img-10.jpeg)
# Conclusion 

- CCNE effort essential to the national cyber mandate:
- CNE situational awareness
- New actor discovery
- Tracking known actors
- Several new actors discovered using this process
- De-confliction needs to be improved
# MM CCNE contacts 

![img-11.jpeg](img-11.jpeg)
