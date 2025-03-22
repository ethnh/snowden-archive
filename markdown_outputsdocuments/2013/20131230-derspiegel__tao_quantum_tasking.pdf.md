# (TS) NSA QUANTUM Tasking Techniques for the R\&T Analyst 

## POC:

TAO RTD | Team |Osteon - Booz Allen Hamilton SDS2

The overall classification of this brief is
TOP SECRET//SI//REL USA, AUS, CAN, GBR, NZL
![img-0.jpeg](img-0.jpeg)
4 (TS//SI//REL) Only R\&T Analysts can submit QUANTUMTHEORY Tasking to the QUANTUM team. TOPI Analysts can submit QUANTUMNATION Tasking through Target Profiler. The biggest difference is QUANTUMTHEORY deploys a stage1 implant called VALIDATOR (soon to be COMMONDEER) and QUANTUMNATION deploys a stage0 implant called SEASONEDMOTH (SMOTH). SMOTHs die within 30 days of deployment unless requested to extend the life.

4 (TS//SI//REL) This presentation does not cover FAA QUANTUM, but if you identify an active selector, compare the SIGAD in Marina to the SIGAD on the GO QUANTUM wiki page to see if FAA QUANTUM is an option.

4 (TS//SI//REL) This presentation is geared towards targets seen at US-20KI. If you are unfamiliar with this SIGAD, it is equivalent to a TS//NF SIGAD that cannot be mentioned in this PowerPoint. You can contact the POC of this brief for more information.
# Web Browsing (Exploit with QUANTUM 

- The concept man-on-the-side)
- QUANTUM is a man-on-the-side capability. If your target has a selector that is active in the last 14 days, vulnerable to the QUANTUM technique, and seen by an SSO site that has QUANTUM capabilities, then there might be the opportunity to detect that communication in real-time and piggy back with the requested content back into the target's network and implant the host.
- QUANTUMTHEORY can be used only if a TAO Project is set up (must coordinate with your R\&T Analyst)
- QUANTUMNATION can be used regardless of a TAO Project (TOPI does the tasking in Target Profiler)
- The biggest difference is QUANTUMTHEORY deploys a stage1 implant called VALIDATOR (soon to be COMMONDEER) and QUANTUMNATION deploys a stage0 implant called SEASONEDMOTH (SMOTH). SMOTHs die within 30 days of deployment unless requested to extend the life. The exploit technique is the same.
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

![img-1.jpeg](img-1.jpeg)

Target
![img-2.jpeg](img-2.jpeg)

Yahoo's
Web Server
![img-3.jpeg](img-3.jpeg)
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

1. Target logs into his Yahoo account
![img-4.jpeg](img-4.jpeg)

Target
![img-5.jpeg](img-5.jpeg)

Yahoo's
Web Server

SSO Site
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

1. Target logs into his Yahoo account
![img-6.jpeg](img-6.jpeg)
![img-7.jpeg](img-7.jpeg)

SSO Site
2. SSO site sees the

QUANTUM tasked Yahoo
selector's packet and forwards
it to TAO's FOXACID Server
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

4. Yahoo server receives the packet requesting email content
![img-8.jpeg](img-8.jpeg)
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

![img-9.jpeg](img-9.jpeg)
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

![img-10.jpeg](img-10.jpeg)
6. The target's Yahoo webpage is loaded but in the background the FOXACID URL loads which redirects to the FOXACID Exploit Server.
![img-11.jpeg](img-11.jpeg)
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

![img-12.jpeg](img-12.jpeg)
# What is QUANTUM? 

## QUANTUM Generic Animation - High Level of How It Works

![img-13.jpeg](img-13.jpeg)
# QUANTUM Capabilities - NSA 

(TS//SI//REL) NSA QUANTUM has the greatest success against <yahoo>, <facebook>, and Static IP Addresses. New QUANTUM realms are often changing, so check the GO QUANTUM wiki page or the QUANTUM SpySpace page to get more up-to-date news.

NSA QUANTUM is capable of targeting the following realms:

-     - IPv4_public
- alibabaForumUser
- doubleclickID
- emailAddr
- rocketmail
- hi5Uid
- hotmailCID
- linkedin
- mail
- mailruMrcu
- msnMailToken64
- mailruMrcu
- WatcherID
# QUANTUMTHEORY - GCHQ 

If a Partnering Agreement Form (PAF) is set up with GCHQ for the CNO project, then the R\&T Analyst can utilize GCHQ QUANTUMTHEORY to include additional capabilities such as:

- ALIBABA - AOL
- BEBO_EMAIL ・ DOUBLE_CLICK
- FACEBOOK_CUSER ・ GOOGLE_PREFID
- GMAIL ・ HIS
- HOTMAIL ・ LINKEDIN
- MAIL_RU ・ MICROSOFT_MUID
- MICROSOFT_ANONA ・ RAMBLER
- RADIUS ・ SIMBAR
- TWITTER ・ YAHOO_B
- YAHOO_L/Y ・ YANDEX_EMAIL
- YOUTUBE ・ IP Address

More information on: https://wiki.gchq/4499_99/QUANTUM_BISCUIT If you cannot get to the link try: http://www.w360.com/4499/
# QUANTUM SIGDEV - QFDs 

(TS//S//REL) Find all Selectors associated to your target (Yahoo, Yahoo B Cookies, Facebook, Hotmail, etc) using Marina, NSA or GCHQ QFDs.

NSA SATC QFDs:
![img-14.jpeg](img-14.jpeg)

Skip to Step 5 once you have all of your selectors...
# QUANTUM SIGDEV - Marina 

Step 1: Skip to Step 5 if you used the QFDs to identify alternate selectors
4 (TS//SI//REL) If you do not use the GCHQ or NSA QFDs you can use Marina. Run a Marina Selector/Identifier Profile (Federated) search for a 3 month range to look for additional selectors.
![img-15.jpeg](img-15.jpeg)
(TS//S//REL) Once the query finishes, look at the Equivalent IDs section. This will show you other selectors that your target is using. This is determined by linking content (logins/email registrations/etc). It is worth verifying that these are indeed selectors associated to your target. NSA QUANTUM works best against <yahoo> and <facebook>. Although, it is worth making note of a <gmail> selector for possible GCHQ QUANTUM support or for your own notes.
![img-16.jpeg](img-16.jpeg)
4 (TS//S//REL) If your search was on a <yahoo> email address, then click on Machine IDs and look for a recent <yahooBcookie>. YahooBcookie's are unique to a specific computer and can hold other <yahoo> addresses that are being logged into on that computer as long as the user does not clear browser cookies. If you see multiple <yahooBcookie> pick the most recent Last Heard date. Also higher the Num Heard is, the more likely that selector does not change.
![img-17.jpeg](img-17.jpeg)
![img-18.jpeg](img-18.jpeg)
(TS//SI//REL) Since ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) ( ) do a Marina Selector Profile query on it to see if there are additional accounts associated to the target. Remember NSA QUANTUM cannot target the <google> selector.
(TS//SI//REL) You can do this by clicking on the selector, scroll down to Selector Profile, and click Range.
![img-19.jpeg](img-19.jpeg)
# (TS//S//REL) Change the query to search for the last 3 Months and click SUBMIT 

![img-20.jpeg](img-20.jpeg)
4 (TS//SI//REL) Once the query finishes, look at the Equivalent IDs section and make note of any new <yahoo>, <hotmail>, <yahooBcookie>, and <facebook> selectors and do the same process to identify additional selectors.

![img-21.jpeg](img-21.jpeg)
(TS//SI//REL) Once you have a list of your selector(s), you will want to look at each one separately to check for the likelihood of successfully exploiting your target via NSA QUANTUM. We are checking to see if the target itself is seen at US- $\$ 0 \%$ and if it is active.
(TS//SI//REL) First we want to run a Marina Active User/Presence (Federated) search on
<facebook> for the past 14 days.
![img-22.jpeg](img-22.jpeg)
4 (TS//SI//REL) You will either have results or not have results. The key is to look at the SIGAD for the results and if the SIGAD is capable of doing QUANTUM then you most likely have a vulnerable target! To check for SIGADs that NSA and GCHQ QUANTUM can target, type GO QUANTUM in your browser. If GCHQ QUANTUM is needed, then work with your R\&T Analyst to follow the appropriate steps on the wiki to set up a PAF.

- (TSI/SI//REL) You will want to look at the Marina results and make note of the most frequent SIGAD/IP CIDR for each Active User/Presence (Federated) query

1) Selector
a) SIGAD
b) Active User IP CIDR - The CIDR will be added to the TLN's Whitelist.
-A TLN's Whitelist is a list containing the IP CIDRs your target uses. It is where the
FOXACID server will only continue with exploitation if the external IP Address of the target/redirection is on the Whitelist for the TLN your R\&T Analyst requests.
# Is My Selector Tasked for QUANTUM? 

If you sent your R\&T analyst a selector to task for QUANTUMTHEORY and you want to see if it has been tasked yet, you can enter the selector in Target Profiler and if you see "tasked for survey" and the Technique to be QUANTUMTHEORY or QUANTUMNATION then it is tasked! You can also see when the last FOXACID redirection took place.
![img-23.jpeg](img-23.jpeg)
# QUANTUMNATION 

QUANTUMNATION uses new TAO CNE tradecraft and automation to drive broad scale initial access, specifically an SSG cloud-analytic to identify selectors in SSO passive collection that are viable for end-point access, and the use of lightweight CNE implants to obtain initial access and survey data delivered to the TOPI offices via corporate SIGINT repositories. For More Information on QUANTUMNATION check the QUANTUMNATION wiki page

Target Profiler now shows if a selector is vulnerable to a QUANTUM exploit. If your target is valid for QUANTUMNATION, A "Vulnerable" link in Target Profiler will appear. Simply click the link that sends an email to request QUANTUMNATION tasking.
![img-24.jpeg](img-24.jpeg)

Note: QUANTUMNATION and standard QUANTUM tasking results in the same exploitation technique. The main difference is QUANTUMNATION deploys a stage 0 implant and is able to be submitted by the TOPI. Any ios device will always get VALIDATOR deployed.
4 (TS//SI//REL) Once you have a selector, SIGAD, and IP CIDR, you are ready to start the process for a FOXACID TLN and Tag request.

4 (TS//SI//REL) Depending on the teams, either an R\&T analyst or the Branch Chief can create a TLN (Twisty Lobby Number). Contact your Branch Chief for information on creating a TLN for each selector you want to target.

4 (TS//SI//REL) Note: You will need 1 TLN and 1 FOXACID Tag per selector you task with QUANTUM.
# Step 8: 

- (TSI/SII/REL) Once you have a TLN, you will need to submit a FOXACID Tag request.
- (TSI/SII/REL) Go to https:/nsa/cgi-bin/ and fill out the appropriate information in the top and within the body of the ticket update this information accordingly. Here is an example:

CT or Non-CT: Non-CT
Second Party/Partnering: No
Country Region/Type: $\square$
FISA Target: No
Type of Op: QUANTUM
Utilizing WPTT: No
Proiect Name: $\square$
TLN: $12345^{\text {® }}$ Insert Your TLN
IP Range: $\square$ Insert Your Active User IP CIDR / WHITELIST
MAC Addresses: Unknown
Payload Requested: Vai
Start Date: 20130401
POCs:
MSO Support: No
4 (TS//SI//REL) Once the ticket is completed, you will receive an email with the FOXACID Tag for your TLN.
(TS//SI//REL) Go to https://sisint@tifil.ne.gr/nsa.ic.gov/Tr/Trindex.php and fill out the appropriate information in the form to task your selector and tag for QUANTUM.
(TS//SI//REL) Once your selector is tasked for QUANTUM you will see the status changed to complete.
(TS//SI//REL) The last step it to monitor the TLN in FOXSEARCH https://www.rus. nsa . . . to look for redirections and update the plugins or WHITELIST if needed.
(TS//SI//REL) De-task your QUANTUM request when you hook your target!
# n 

4 If you have any questions or comments about this presentation, please send an email to $\square$ at $\qquad$ @nsa.ic.gov
1
