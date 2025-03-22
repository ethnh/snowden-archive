# PRESTON Business Processes 

Version 1.0
![img-0.jpeg](img-0.jpeg)

## Synopsis

The purpose of this document is to present a brief study of the PRESTON Business Processes.

## Chapter

This information is exempt from disclosure under the Freedom of Information Act 2000 and may be subject to exemption under other UK information legislation. Refer disclosure requests to GCHQ on
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

## Distribution

![img-1.jpeg](img-1.jpeg)

## Document Amendment History

| Version | Date | R\&A | Amendments |
| :--: | :--: | :--: | :--: |
| 0.5 | 17 April 2007 | - | Updated following review with PRESTON Ops. |
| 0.6 | 8 May 2007 | Yes | Updated following formal review (reference PRR Sigmod/00184CPO/4502/SIG006 400/16) |
| 1.0 | 8 May 2007 | - | First formal issue |

## Soft Copy References

File References for this document when issued:
vob:/preston/tech/analysis/preston-business-analysis.doc
2 of 24
# SECRET STRAP 1 

PRESTON Business Processes Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

## Contents

1 INTRODUCTION ..... 5
1.1 Objectives ..... 5
1.2 Glossary ..... 5
2 USE CASES ..... 6
2.1 Use-Case Model Overview ..... 6
2.2 Actors ..... 6
2.3 Use cases ..... 6
3 USE CASE: ENABLE INTERCEPTION ..... 7
3.1 Brief description ..... 7
3.2 Basic flow ..... 8
3.3 Alternate flows ..... 8
4 USE CASE: DISABLE INTERCEPTION ..... 10
4.1 Brief description ..... 10
4.2 Preconditions ..... 10
4.3 Basic flow ..... 10
4.4 Further detail ..... 10
5 USE CASE: PRODUCE INTELLIGENCE ..... 11
5.1 Brief description ..... 11
5.2 Preconditions ..... 12
5.3 Basic flow ..... 12
5.4 Alternate flows ..... 12
6 USE CASE ANALYSIS ..... 13
6.1 Enable interception ..... 13
6.2 Produce intelligence ..... 17
6.3 Business Workers and Business Actors ..... 18
6.4 Business Entities ..... 19
# SECRET STRAP 1 

PRESTON Business Processes Sigmod/00003CPO/4502/SIG010900/23
8 May 2007
6.5 Organisational responsibilities ..... 21
7 DERIVED USE CASES ..... 22
7.1 Collection system ..... 22
7.2 Stream routing ..... 23
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

## 1 INTRODUCTION

## 1.1 Objectives

This document presents analysis on the PRESTON business processes. This analysis can be used:

- To understand how business change affects the system.
- To derive requirements for the development.
- To derive test cases to verify the correctness of the development.

The objectives of this document are:

- To present the PRESTON business processes.
- To describe how the business processes are implemented using the PRESTON systems.
- To derive use cases from the business processes.


### 1.2 Glossary

GCHQ Government Communications Headquarters.
NTAC National Technical Assistance Centre.
# 2 USE CASES 

### 2.1 Use-Case Model Overview

The Business Use Case Model for PRESTON is presented in the diagram below.
![img-2.jpeg](img-2.jpeg)

### 2.2 Actors

The Use Case Model describes the following actors:

## Interception authority

Target
Intelligence analyst

The interception authority is responsible for approving the interception warrants placed on targets.
The target is a potential source of intelligence.
The intelligence analyst is responsible for delivering intelligence from intercepted target communications.

### 2.3 Use cases

The Use Case Model describes the following Use Cases:

## Enable interception

Disable interception
Produce intelligence

This use case describes how the Intelligence analyst enables an interception service.
This use case describes how the Intelligence analyst terminates use of an interception service.

This use case describes how an Intelligence analyst produces intelligence from a Target's intercept.

6 of 24
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

## 3 USE CASE: ENABLE INTERCEPTION

![img-3.jpeg](img-3.jpeg)

### 3.1 Brief description

This use case describes how the Intelligence analyst enables an interception service.

7 of 24

This information is exempt from disclosure under the Freedom of Information Act 2000 and may be subject to exemption under other UK information legislation. Refer disclosure requests to GCHQ or
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 3.2 Basic flow

The use case begins when an intelligence analyst wishes to place a target on cover.

## \{Identify communication address\}

The analyst identifies the target's communication address. For some types of communication, it will be necessary to check the subscriber's identity with the Tasking manager, to verify that the communication address is indeed the property of the target.
[Should this include a subscriber check use case?]
The analyst requests a feasibility study describing the communication address.
The analyst initiates drafting of a warrant application in conjunction with the OPPLEG.

## \{Conduct feasibility check\}

A feasibility check is performed, in conjunction with the data provider.
The communication address is added to the warrant schedule.
The warrant is completed, and sent to OPP-LEG.
The warrant is sent to the FCO WLD for approval.

## \{Consider warrant\}

FCO WLD considers the case for the warrant.
The WLD apartment advises GCHQ and the interception capability that interception is approved.
A collection request form [MIDDLESEX GREEN] is prepared for submission.
The communication address is advised to the interception capability and interception begins.
The use case ends.

### 3.3 Alternate flows

3.3.1 No intention to target

At \{Identify communication address\}, if there is no intention to target based on information gained.

The use case ends.

### 3.3.2 Not feasible to intercept

At \{Conduct feasibility check\} if the interception is not feasible.
# SECRET STRAP 1 

The use case ends.

### 3.3.3 Warrant not approved

At \{Consider warrant\}, if the case for warranty is not strong enough.
The use case ends.

9 of 24

This information is exempt from disclosure under the Freedom of Information Act 2000 and may be subject to exemption under other UK information legislation. Refer disclosure requests to GCHQ or
# 4 USE CASE: DISABLE INTERCEPTION 

![img-4.jpeg](img-4.jpeg)

Intelligence analyst

Disable interception
![img-5.jpeg](img-5.jpeg)

### 4.1 Brief description

This use case describes how the Intelligence analyst terminates use of an interception service.

### 4.2 Preconditions

- Target intercept has been enabled.


### 4.3 Basic flow

The use case begins when an Intelligence analyst wishes to terminate use of an interception warrant.

The Intelligence Analyst notifies the tasking authority that the interception is to be terminated.

The interception capability is de-tasked, and intercept ceases.
The use case ends.

### 4.4 Further detail

There is a follow-up legal process involving OPP-LEG and FCO/WLD where the number(s) are formally removed from the warrant schedule (or the whole warrant is cancelled).

## SECRET STRAP 1
# 5 USE CASE: PRODUCE INTELLIGENCE 

![img-6.jpeg](img-6.jpeg)
![img-7.jpeg](img-7.jpeg)

### 5.1 Brief description

This use case describes how an Intelligence analyst produces intelligence from a Target's intercept.
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 5.2 Preconditions

- The communication address has been targeted.
- The interception capability has been tasked as a result of a warrant.


### 5.3 Basic flow

The use case begins when a target communicates using a communication address which is on cover.
The target communicates using an intercepted communication resource.
The interception capability intercepts the communication, and forwards the intercept to the interception reception centre, where the intercept is processed and forwarded to the Intelligence analyst.
The Intelligence analyst reviews the communications intercept,

## \{Derive intelligence\}

The intelligence analyst analyses the communication and derives information which may be of intelligence value.
The Intelligence analyst issues intelligence as intelligence reports.
The use case ends.

### 5.4 Alternate flows

5.4.1 Intercept not reportable

At \{Derive intelligence\} if the communication intercept contains no intelligence.
The use case ends.
# 6 USE CASE ANALYSIS 

This section looks at the most significant Business Use Cases, and scenarios which realise those use cases.

### 6.1 Enable interception

The Enable interception use case is commonly implemented in one of two ways. Either:

- The intercept source is delivered to SD for analysis, before being tasked for operational collection. I use 3 scenarios to describe this process: Enable delivery, Perform survey, Migrate to collection.
- The intercept source is well understood and can be immediately tasked for operational collection. The Enable delivery and Enable collection scenarios are used.


### 6.1.1 Enable delivery

The initial enabling of the intercept source is illustrated using the sequence diagram below. The diagram introduces two new roles:

## Interception capability

The interception capability provides the means to intercept a target's communications. Interception is normally possible when empowered by an approved warrant.

## Tasking manager

The Tasking manager is responsible for ensuring the continuing delivery of intercept derived from warrants from the Target to the Intelligence analyst.

The Interception capability describes the interception role, which is usually performed by the CSPs on our behalf - once we have presented them with a warrant. The Interception capability is sometimes owned by NTAC, and is available as a service to us (again, a warrant is required to use the service).
The Tasking manager is responsible for all communication with the CSP or NTAC on behalf of the Intelligence Analyst.
# SECRET STRAP 1 

![img-8.jpeg](img-8.jpeg)

This scenario describes how the intercept is enabled only. At this stage, no tasking is applied, nor is the intercept routed to a particular location. The Tasking manager ensures that the intercept is delivered correctly.

### 6.1.2 Perform survey

For the Perform survey scenario, two new roles are introduced:

## Stream routing

SD analyst

The Stream rouing is responsible for delivery of intercept to the appropriate party for processing.

The SD analyst is responsible for maintaining an understanding of the Target's communication technology, and ensuring that the system can continue to process the Target's communications.

The Tasking Manager manages the routing of the intercept to the SD analyst using 14 of 24

[^0]
[^0]:    The St
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007
the Stream routing function.
![img-9.jpeg](img-9.jpeg)

The SD analyst performs a survey and provides the Intelligence analyst with information to allow them to Assess the intelligence value of the new intercept source.

If the signal is going to be tasked for operational collection, the SD analyst also develops a processing configuration which will allow the intercept source to be tasked operationally.

### 6.1.3 Migrate to collection

For this scenario, I introduce 3 new roles:
System administrator The System Administrator is responsible for maintaining the processing systems to ensure their continued contribution to the interception process.
Collection manager
The Collection manager is responsible for ensuring the continued delivery of processed intercept items from raw intercept.
Collection system
The collection system is responsible for processing a target's raw intercept and delivering the processed intercept items to an Intelligence Analyst, thus enabling them to produce intelligence.

The Tasking manager manages the migration of the intercept source to operational collection tasking.

15 of 24

[^0]
[^0]:    This information is exempt from disclosure under the Freedom of Information Act 2000 and may be subject to exemption under other UK information legislation. Refer disclosure requests to GCHQ or
# SECRET STRAP 1 

![img-10.jpeg](img-10.jpeg)

The System Administrator migrates the tasking configuration to the operational system. The Collection manager manages the Collection system, and so is responsible for addition of the processing task, along with day-to-day monitoring of the task.
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 6.1.4 Enable collection

This scenario describes how the intercept source is enabled for operational collection with a survey stage. The Tasking manager manages this migration - this scenario is very similar to the Migrate to collection scenario.
![img-11.jpeg](img-11.jpeg)

### 6.2 Produce intelligence

![img-12.jpeg](img-12.jpeg)

This scenario illustrates how the Interception capability, Stream routing and Collection system collaborate to deliver intercept to the Intelligence analyst.

17 of 24
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 6.3 Business Workers and Business Actors

![img-13.jpeg](img-13.jpeg)

The roles identified can be represented as Business Workers in RUP (Rational Unified Process). The diagram above shows the Business Actors and Business Workers along with their roles. An association is shown between Actors and Workers which interact.
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 6.4 Business Entities

![img-14.jpeg](img-14.jpeg)

Business entities represent ways in which the business stores and exchanges information in order to do its work. The diagram above introduces three Business Entities.

## Stream route

## Collection task

Processing task

A stream route describes an instruction to deliver intercept to a particular intercept processing function.

A collection task describes an intercept collection task at a high level. It describes the target's details, the resources to use, and the configuration to use.

The Processing task describes an instruction to a Collection system to process intercept.

The Stream route is used to route a PRESTON intercept source from its point of reception at GCHQ to its processing location. No processing occurs on the intercept stream until it is routed to its correct location. E.g. a task on the TERRAIN system, or to an analyst performing offline analysis.
The Processing task is a low-level processing instruction for a Collection system to process a source of intercept. The Collection task is a high-level instruction, and is used to communicate operational tasking information from the Tasking manager to the Collection manager e.g. a task on HANGER LANE.
# SECRET STRAP 1 

![img-15.jpeg](img-15.jpeg)

The Warrant schedule and Warrant entities are shown in the above diagram.

## Warrant

A warrant names the target and states the purpose(s) for which the warrant has been issued. It is usually issued by a Secretary of State. In exceptional circumstances it may be issued by a senior official, providing this has been expressly authorised by a Secretary of State.

Warrant schedule A warrant schedule lists the selection factors which can be used in the interception. A warrant can have a number of schedules.
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 6.5 Organisational responsibilities

![img-16.jpeg](img-16.jpeg)

Most of the roles discussed here are specific to GCHQ's business. NTAC's service is the provision of the interception capability. Currently, the roles are fulfilled thus:

## Interception capability

## System administrator

SD analyst

Collection manager
Stream routing
Collection system

Tasking manager

This is a service which CSPs are mandated to provide under RIPA. NTAC manages the delivery of these services for all UK agencies.
This role is fulfilled by TSS-ISS for PRESTON.
OPD-GTE are mainly responsible for survey of PRESTON data, but this role is also shared with SD staff at Bude or Scarborough to share the load.
This role is fulfilled by GSOC who provide 24hr monitoring of the collection systems.
The NHIS router product provides this function.
The TERRAIN product performs processing for PRESTON.

PRESTON OPS (CADWELL PARK) manage PRESTON tasking.
# 7 DERIVED USE CASES 

### 7.1 Collection system

The following section briefly describes the Use Cases which apply to the Collection system.
![img-17.jpeg](img-17.jpeg)

The following Use Cases are derived:

| Begin stream <br> processing | This use case describes how the Collection manager <br> initiates processing of an intercept stream. |
| :-- | :-- |
| End stream processing | This use case describes how the Collection manager <br> terminates processing of an intercept stream. |
| Process intercept | This use case describes how the stream routing <br> function delivers intercept to the Collection system for <br> processing, and delivery to the Intelligence analyst. |

The following actors have been defined previously:
Collection manager The Collection manager is responsible for ensuring the continued delivery of processed intercept items from raw intercept.
Stream routing The Stream routing is responsible for delivery of intercept to the appropriate party for processing.
Intelligence analyst The intelligence analyst is responsible for delivering intelligence from intercepted target communications.
# SECRET STRAP 1 

PRESTON Business Processes
Sigmod/00003CPO/4502/SIG010900/23
8 May 2007

### 7.2 Stream routing

The following section briefly describes the Use Cases which apply to the Stream routing.
![img-18.jpeg](img-18.jpeg)

The following Use Cases are derived:

## Add stream route

Delete stream route

Modify stream route

Route intercept

This use case describes how a Tasking manager adds a new stream route instruction to the Stream routing's routing table.
This use case describes how a Tasking manager deletes an existing stream route instruction from the Stream routing's routing table.
This use case describes how a Tasking manager modifies an existing stream route instruction in the Stream routing's routing table.
This use case describes how the Stream routing routes intercept received from the Interception capability to the appropriate Collection system in accordance with the routing instructions.

The following actors have been defined previously:
Tasking manager
The Tasking manager is responsible for ensuring the continuing delivery of intercept derived from warrants from the Target to the Intelligence analyst.

## SECRET STRAP 1
# SECRET STRAP 1 

## 8 May 2007

## Interception capability

## Collection system

The interception capability provides the means to intercept a target's communications. Interception is normally possible when empowered by an approved warrant.

The collection system is responsible for processing a target's raw intercept and delivering the processed intercept items to an Intelligence Analyst, thus enabling them to produce intelligence.
