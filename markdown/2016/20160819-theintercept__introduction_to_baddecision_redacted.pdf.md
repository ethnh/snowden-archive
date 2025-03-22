# Introduction to BADDECISION 

December 15-16, 2010
# Classification 

## The overall classification of this presentation is TOP SECRET//COMINT//NOFCERN

All slides and materiels contained in this presentation should be considered classified TS/Sl/NF (unless otherwise noted)
# Section Overview 

## $>$ BADDECISION Overview <br> $>$ BADDECISION Components <br> $>$ BADDECISION Prerequisites <br> $>$ BADDECISION Operational Flow <br> $>$ BADDECISION Step Through <br> $>$ Instructor-led Demos and Labs <br> $>$ BADDECISION Pros / Cons
# At The End... 

You should be able to....
$>$ Understand BADDECISION Components
$>$ Understand the BADDECISION Prereqs.
$>$ Conduct a BADDECISION Operation.
$>$ List the Pros / Cons of NIGHTSTAND.
# BADDECISION Overview 

## $>$ BADDECISION is an "802.11 CNE tool that uses a true man-in-the-middle attack and a frame injection technique to redirect a target client to a FOXACID server."

Takes advantage of shared open medium and the HTTP protocol.
$>$ Works for WPA / WPA2!
# BADDECISION Prerequisites 

## Working BLINDDATE Survey!

> Client on the Target network
$>$ Security Level: WPA / WPA2
$>$ Ability to maintain a reliable connection to a target network.
$>$ Don't forget FOXACID Tag!
# BADDECISION Components 

## $>$ HAPPYHOUR <br> $>$ SECONDDATE <br> $>$ Open Sources Tools <br> $>$ macchanger <br> $>$ wireshark <br> $>$ nmap <br> $>$ ettercap
# BADDECISION Preparation 

![img-0.jpeg](img-0.jpeg)
# BADDECISION Preparation 

![img-1.jpeg](img-1.jpeg)
# BADDECISION Preparation 

![img-2.jpeg](img-2.jpeg)
# BADDECISION Preparation 

![img-3.jpeg](img-3.jpeg)
# BADDECISION Preparation 

![img-4.jpeg](img-4.jpeg)
# BADDECISION Preparation 

![img-5.jpeg](img-5.jpeg)
# BADDECISION Preparation 

![img-6.jpeg](img-6.jpeg)
# BADDECISION Preparation 

![img-7.jpeg](img-7.jpeg)
# BADDECISION Preparation 

![img-8.jpeg](img-8.jpeg)
# BADDECISION Preparation 

![img-9.jpeg](img-9.jpeg)
# BADDECISION Preparation 

![img-10.jpeg](img-10.jpeg)
# Overview of Operational Scenario 

## $>$ Operator with BLINDDATE

System.
$>$ FOXACID Tag issued for Target.
$>$ Target Client browsing the Internet via web browser (3)
![img-11.jpeg](img-11.jpeg)
# Webpage Request 

Target issues HTTP GET Request to webpage of interest (cnn.com)
![img-12.jpeg](img-12.jpeg)
## Injection

> Operate uses SECONDDATE to inject a redirection payload at Target Client.

Target Client's original HTTP GET Request continues on it's normal path.
![img-13.jpeg](img-13.jpeg)
# Refresh and Covert Request 

## - Injected payload forces Target Client to refresh and send another HTTP GET Request to desired webpage. <br> - Covert Request is issued by Target Client to FOXACID Server.

![img-14.jpeg](img-14.jpeg)
## FOXACID

Request Received

## FOXACID

receives request from entity.
Entity is
validated as Target
Client by FOXACID Tag.

Response to original HTTP GET Request is dropped (but don't worry, that's good)
![img-15.jpeg](img-15.jpeg)
# FOXACID 

Browser Survey

- FOXACID Server instantiates browser survey on Target Client to detect vulnerabilities.
![img-16.jpeg](img-16.jpeg)
# FOXACID 

Browser Survey

- FOXACID Server instantiates browser survey on Target Client to detect vulnerabilities.
![img-17.jpeg](img-17.jpeg)
## Survey, Payload, Exploitation

## Covert

communicates continue between FOXACID and Target until found not vulnerabilities or exploited.

## > Target Client

continues normal webpage browsing, completely unaware
(c)
![img-18.jpeg](img-18.jpeg)
# WHACKED! 

That's the ultimate goal.
![img-19.jpeg](img-19.jpeg)
# BADDECISION Step Through 

## $>$ Let's go through this together...

$>$... because there are many more pieces!
# BADDECISION Demos and Labs 

## Grab a partner!

> One Target Client, one Operator.
> Have fun getting whacked!
# BADDECISION Pros / Cons 

## Pros

Works for WPA / WPA2 networks.
Can reliability see all communications between target and FOXACID.

## $>$ Cons

Larger signature than NIGHTSTAND.
$>$ Requires higher SNR to maintain reliable communications between target and FOXACID.
# The End. 

## Questions?
