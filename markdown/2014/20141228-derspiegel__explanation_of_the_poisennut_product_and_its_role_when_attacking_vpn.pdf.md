# (U) Template:POISONNUT Product 

From WikiInfo

## Contents

- 1 (TS//REL) Overview
- 2 (TS//REL) Design
- 3 (TS//REL) Capabilities
- 3.1 (TS//REL) Can Attack
- 3.2 (TS//REL) Submit Attack
- 3.3 (TS//REL) Submission to Output Correlator
- 3.4 (TS//REL) Cancel Attack
- 3.5 (TS//REL) Attack Output Processor
- 3.6 (TS//REL) Was Attack Successful
- 4 (U//FOUO) Infrastructure
- 4.1 (U//FOUO) Channel Guide
- 5 (U//FOUO) Metrics
- 6 (U//FOUO) Issues


## (TS//REL) Overview

- (TS//REL) Description: This complex element is responsible for scheduling ESP attacks.
- (U//FOUO) Input Channel(s): incomingESPAttack
- (S//REL) Output Channel(s): successfulESPAttack (successful attack)
- See the pinpoint photographing-phenotrack Maven Project.


## (TS//REL) Design

![img-0.jpeg](img-0.jpeg)

## (TS//REL) Capabilities

## (TS//REL) Can Attack

- (TS//REL) Description: Determines if the data that is available for the Phase1 Attack is enough to do the current attack in the attack plan. If it is not, it sets the result text and returns the cannotAttack route. The strategy is not marked as failed, this is left for the object on the other side of the channel to decide how to handle the failure. If no plan is set or the plan has no attacks, it returns the cannotAttack route. If there are strategies but all of them have been exhausted, the plan will throw an IllegalStateException.


## (TS//REL) Submit Attack

- (TS//REL) Description: Creates the Attack command and submits it to the VRI with the Resource of the Attack Strategy. The VRI correlation id must be set with the Phase1 data.


## (TS//REL) Submission to Output Correlator

- (TS//REL) Description: Correlates the Phase1 with it's VRI Output. The VRI Correlation id will be used for the correlation. There will be a time out on the phase1 that will indicate that we never got the VRI Output.
# Template:POISONNUT Product - WikiInfo 

## (TS//REL) Cancel Attack

- (TS//REL) Description: Sends a message to the VRI that the job has been canceled.


## (TS//REL) Attack Output Processor

- (TS//REL) Description: Processes the output of the Attack. This output may not even be there if the Attack timed out. The Attack Strategy needs to be marked as successful or failed based on the data the Attack gives back.


## (TS//REL) Was Attack Successful

- (TS//REL) Description: Checks to see if the current Attack Strategy was successful. This component could use the Has Phase1 Key Material Content Based Router implementation with a different input channel/output channel configuration.


## (U//FOUO) Infrastructure

## (U//FOUO) Channel Guide

| Channel | Name | Type | Payload |
| :--: | :--: | :--: | :--: |
| CanAttack Input 1 (Channel L) | incomingPhaseAttack | Direct | KE Phase1 |
| CanAttack Output 1 | canAttackPhase1 | Direct | KE Phase1 |
| CanAttack Output 2 | cannotAttackPhase1 | Direct | KE Phase1 |
| RequestResponseCorrelator Input 1 | attackRequestSubmitted | Direct | VRISubmission |
| RequestResponseCorrelator Input 2 | attackResponseReceived | Direct | VRIResponse |
| RequestResponseCorrelator Output 1 | attackCompleted | Direct | VRISubmission |
| RequestResponseCorrelator Output 2 | attackTimedOut | Direct | VRISubmission |

## (U//FOUO) Metrics

$\{\{($ metrics $\}\}\}$

## (U//FOUO) Issues

$\{\{($ issues $\}\}\}$

Retrieved from
Category: POISONNUT products
Derived From: 70 Classופ Curl: 20-01. DAN: 70100701
and US\&C/2014: 07. DAN: 70170110
Southeast: 09. 2010010
