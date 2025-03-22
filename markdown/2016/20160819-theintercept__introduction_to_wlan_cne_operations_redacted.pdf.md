# Introduction to WLAN / 802.11 Active CNE Operations 

December 15-16, 2010
# Classification 

## The overall classification of this presentation is TOP SECRET//COMINT//NOFCERN

All slides and materiels contained in this presentation should be considered classified TS/Sl/NF (unless otherwise noted)
# Section Overview 

## $>$ Passive to Active Operations <br> > WLAN CNE Criteria / Assessment <br> $>$ Active CNE Operations <br> $>$ Introduction to FOXACID
# At The End... 

You should be able to...
$>$ Identify Criteria for CNE Assessment.
$>$ List the Active CNE Operational Process
$>$ Describe the purpose of FOXACID.
# Passive to Active Operations 

$>$ Primary Goal: To enable on-net access to target networks via off-net capabilities.
$>$ Prerequisite: We need to find the network of interest in order to target it.
$>$ Procedure: Conduct passive survey to locate network, then perform active op.
$>$ Solution: Utilize BLINDDATE and the appropriate plug-in solution(s).
# Passive to Active Operations 

## $>$ Successful operation of BLINDDATE is essential to correct usage of plug-ins. <br> $>$ Two types of plug-ins exist: <br> $>$ Analysis Tool Aids <br> $>$ Active CNE Tools <br> $>$ We will focus on Active CNE Tools: <br> $>$ NIGHTSTAND <br> $>$ HAPPYHOUR
# Active CNE Assessment 

## $>$ BLINDDATE used as both a survey and vulnerability analysis tool for 802.11 networks.

$>$ Operator needs to know what vulnerabilities, or criteria, to look for in order to utilize the correct Active CNE Tool (if any) $>$ We will focus primarily on criteria necessary to carry out NIGHTSTAND (NS) and BADDECISION (BDN) operations.
# Major Assessment Criteria 

## $>$ Clients

$>$ A client is a prerequisite: If no clients are on the target network, there's nothing to do yet.

## $>$ Security

$>$ Encryption setting (Open, WEP, WPA, WPA2) dictates which capability can be used (if any).

## Signal Strength

$>$ SNR dictates whether we can perform a successful active CNE operation.
# Active CNE Operations 

## $>$ What is our end goal?

$>$ Provide on-net access via off-net means.
$>$ How do we do that?
$>$ Redirect the target to the TAO infrastructure.
$>$ How do we do that?
$>$ Inject payload destined for the target client.
# Active CNE Operations 

## $>$ What does that do exactly?

$>$ Forces the target to covertly contact a FOXACID server.
What is FOXACID suppose to do?
Perform vulnerability analysis and exploitation of the target (if possible).
# Introduction to FOXACID 

## $>$ FOXACID is the cover term for a DNT/ROC project to deliver content based exploits (CBE) to web browsers. <br> $>$ The greatest vulnerability to your computer: your web browser.
# Introduction to FOXACID 

## $>$ FOXACID Servers sit on Internet. <br> $>$ Publicly addressable, DNS resolved. <br> $>$ Utilizes whitelist for security, filtering. <br> $>$ Requires specially crafted URL tag to contact FA Servers (FOXACID Tag).
# Example Tag 

http://Domain/PluginName/PluginName2/ .istBegin/Group/ListEnd/DeploymentIDTLN_MSGID.html http://oaseball2.2ndhallplays.com/nested/ attrib/simc/11d87inc/forms9952_21222.html
# FOXACID Tags 

- Designed to look ambiguous.
- Unique for a particular target / operation.
- All fields in the tag denote something special...
# Redirection to FOXACID 

## > A FOXACID Tag is a special URL pointing to a particular FOXACID Server. <br> $>$ Contacting the FA Server will (hopefully) result in the contactor being exploited. <br> $>$ We want the target to be exploited. <br> $>$ How do we redirect the target to the FOXACID Server without being noticed. <br> $>$ Use NIGHTSTAND or BADDECISION
# The End. 

## Questions?
