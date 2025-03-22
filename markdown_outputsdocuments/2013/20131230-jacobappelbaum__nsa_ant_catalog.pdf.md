![img-0.jpeg](img-0.jpeg)

# DEITYBOUNCE 

## ANT Product Data

(TSI/SI/IREL) DEITYBOUNCE provides software application persistence on Dell PowerEdge servers by exploiting the motherboard BIOS and utilizing System Management Mode (SMM) to gain periodic execution while the Operating System loads.
![img-1.jpeg](img-1.jpeg)
(TSI/SI/IREL) DEITYBOUNCE Extended Concept of Operations
(TSI/SI/IREL) This technique supports multi-processor systems with RAID hardware and Microsoft Windows 2000, 2003, and XP. It currently targets Dell PowerEdge 1850/2850/1950/2950 RAID servers, using BIOS versions A02, A05, A06, 1.1.0, 1.2.0, or 1.3.7.
(TSI/SI/IREL) Through remote access or interdiction, ARKSTREAM is used to reflash the BIOS on a target machine to implant DEITYBOUNCE and its payload (the implant installer). Implantation via interdiction may be accomplished by nontechnical operator though use of a USB thumb drive. Once implanted, DEITYBOUNCE's frequency of execution (dropping the payload) is configurable and will occur when the target machine powers on.

Status: Released / Deployed. Ready for
Unit Cost: $\$ 0$ Immediate Delivery

POC: $\square$ S32221, $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ?
![img-2.jpeg](img-2.jpeg)

# IRONCHEF 

## ANT Product Data

(TS//SI//REL) IRONCHEF provides access persistence to target systems by exploiting the motherboard BIOS and utilizing System Management Mode (SMM) to communicate with a hardware implant that provides two-way RF communication.
![img-3.jpeg](img-3.jpeg)
(TS//SI//REL) IRONCHEF Extended Concept of Operations
(TS//SI/REL) This technique supports the HP Proliant 380DL G5 server, onto which a hardware implant has been installed that communicates over the $I^{2} \mathrm{C}$ Interface (WAGONBED).
(TS//SI//REL) Through interdiction, IRONCHEF, a software CNE implant and the hardware implant are installed onto the system. If the software CNE implant is removed from the target machine, IRONCHEF is used to access the machine, determine the reason for removal of the software, and then reinstall the software from a listening post to the target system.

Status: Ready for Immediate Delivery
Unit Cost: $\$ 0$
POC: $\square$ S32221, $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ?
![img-4.jpeg](img-4.jpeg)
![img-5.jpeg](img-5.jpeg)

# GOURMETTROUGH 

## ANT Product Data

(TS//SI//REL) GOURMETTROUGH is a user configurable persistence implant for certain Juniper firewalls. It persists DNT's BANANAGLEE implant across reboots and OS upgrades. For some platforms, it supports a minimal implant with beaconing for OS's unsupported by BANANAGLEE.
![img-6.jpeg](img-6.jpeg)
(TSI/StI/REL) GOURMETTROUGH Persistence Implant Concept of Operations
(TSI/SI//REL)For supported platforms, DNT may configure BANANAGLEE without ANT involvement. Except for limited platforms, they may also configure PBD for minimal implant in the case where an OS unsupported by BANANAGLEE is booted. Status: GOURMETTROUGH is on the shelf and has been deployed on many target platforms. It supports nsg5t, ns50, ns25, isg1000(limited). Soon- ssg140, $\mathrm{ssg5}, \mathrm{ssg} 20$

Unit Cost: $\$ 0$

POC: S32222, $\square$ nsa.ic.gov
![img-7.jpeg](img-7.jpeg)

# HALLUXWATER ANT Product Data 

(TS//SI//REL) The HALLUXWATER Persistence Back Door implant is installed on a target Huawei Eudemon firewall as a boot ROM upgrade. When the target reboots, the PBD installer software will find the needed patch points and install the back door in the inbound packet processing routine.
![img-8.jpeg](img-8.jpeg)
(TS/ISI/IREL) HALLUXWATER Persistence Implant Concept of Operations
(TS/ISI/IREL) Once installed, HALLUXWATER communicates with an NSA operator via the TURBOPANDA Insertion Tool (PIT), giving the operator covert access to read and write memory, execute an address, or execute a packet.
(TS/ISI/IREL) HALLUXWATER provides a persistence capability on the Eudemon 200, 500, and 1000 series firewalls. The HALLUXWATER back door survives OS upgrades and automatic bootROM upgrades.

Status: (U//FOUO) On the shelf, and has been deployed.
POC: $\square$ S32222, $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$
![img-9.jpeg](img-9.jpeg)

# JETPLOW <br> ANT Product Data 

(TS//SI//REL) JETPLOW is a firmware persistence implant for Cisco PIX Series and ASA (Adaptive Security Appliance) firewalls. It persists DNT's BANANAGLEE software implant. JETPLOW also has a persistent back-door capability.
![img-10.jpeg](img-10.jpeg)
(TSI/SI//REL) JETPLOW Persistence Implant Concept of Operations
(TSI/SI//REL) JETPLOW is a firmware persistence implant for Cisco PIX Series and ASA (Adaptive Security Appliance) firewalls. It persists DNT's BANANAGLEE software implant and modifies the Cisco firewall's operating system (OS) at boot time. If BANANAGLEE support is not available for the booting operating system, it can install a Persistent Backdoor (PBD) designed to work with BANANAGLEE's communications structure, so that full access can be reacquired at a later time. JETPLOW works on Cisco's 500-series PIX firewalls, as well as most ASA firewalls (5505, 5510, 5520, 5540, 5550).
(TSI/SI//REL) A typical JETPLOW deployment on a target firewall with an exfiltration path to the Remote Operations Center (ROC) is shown above. JETPLOW is remotely upgradeable and is also remotely installable provided BANANAGLEE is already on the firewall of interest.

Status: (C//REL) Released. Has been widely deployed. Current availability restricted based on OS version (inquire for details).

[^0]
[^0]:    POC: $\square$ S32222, $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ ? $\square$ Derived From: NSACSSM 1-52

    Dated: 20070108
    Declassify On: 20320108
![img-11.jpeg](img-11.jpeg)
![img-12.jpeg](img-12.jpeg)

# HEADWATER <br> ANT Product Data 

(TS//SI//REL) HEADWATER is a Persistent Backdoor (PBD) software implant for selected Huawei routers. The implant will enable covert functions to be remotely executed within the router via an Internet connection.
![img-13.jpeg](img-13.jpeg)
(TSI/SI//REL) HEADWATER Persistence Implant Concept of Operations
(TS//SI//REL) HEADWATER PBD implant will be transferred remotely over the Internet to the selected target router by Remote Operations Center (ROC) personnel. After the transfer process is complete, the PBD will be installed in the router's boot ROM via an upgrade command. The PBD will then be activated after a system reboot. Once activated, the ROC operators will be able to use DNT's HAMMERMILL Insertion Tool (HIT) to control the PBD as it captures and examines all IP packets passing through the host router.
(TS//SI//REL) HEADWATER is the cover term for the PBD for Huawei Technologies routers. PBD has been adopted for use in the joint NSA/CIA effort to exploit Huawei network equipment. (The cover name for this joint project is TURBOPANDA.)

Status: (U//FOUO) On the shelf ready for deployment.
POC: S32222, $\square$ ensa.ic.gov
![img-14.jpeg](img-14.jpeg)
![img-15.jpeg](img-15.jpeg)

# SIERRAMONTANA 

## ANT Product Data

(TS//SI//REL) SIERRAMONTANA provides persistence for DNT implants. The DNT implant will survive an upgrade or replacement of the operating system - including physically replacing the router's compact flash card.
![img-16.jpeg](img-16.jpeg)
(TS//SI//REL) Currently, the intended DNT Implant to persist is VALIDATOR, which must be run as a user process on the target operating system. The vector of attack is the modification of the target's BIOS. The modification will add the necessary software to the BIOS and modify its software to execute the SIERRAMONTANA implant at the end of its native System Management Mode (SMM) handler.
(TS//SI//REL) SIERRAMONTANA must support all modern versions of JUNOS, which is a version of FreeBSD customized by Juniper. Upon system boot, the JUNOS operating system is modified in memory to run the implant, and provide persistent kernel modifications to support implant execution.
(TS//SI//REL) SIERRAMONTANA is the cover term for the persistence technique to deploy a DNT implant to Juniper M-Series routers.

## Unit Cost: $\$$

Status: (U//FOUO) SIERRAMONTANA under development and is expected to be released by 30 November 2008.

[^0]
[^0]:    POC: U//FOUO
    S32222.
    S32222.
    $\square$ ensa.gov
![img-17.jpeg](img-17.jpeg)

# STUCCOMONTANA ANT Product Data 

(TS//SI//REL) STUCCOMONTANA provides persistence for DNT implants. The DNT implant will survive an upgrade or replacement of the operating system including physically replacing the router's compact flash card.
![img-18.jpeg](img-18.jpeg)
(TS//SI//REL) Currently, the intended DNT Implant to persist is VALIDATOR, which must be run as a user process on the target operating system. The vector of attack is the modification of the target's BIOS. The modification will add the necessary software to the BIOS and modify its software to execute the STUCCOMONTANA implant at the end of its native System Management Mode (SMM) handler.
(TS//SI//REL) STUCCOMONTANA must support all modern versions of JUNOS, which is a version of FreeBSD customized by Juniper. Upon system boot, the JUNOS operating system is modified in memory to run the implant, and provide persistent kernel modifications to support implant execution.
(TS//SI//REL) STUCCOMONTANA is the cover term for the persistence technique to deploy a DNT implant to Juniper T-Series routers.

## Unit Cost: $\$$

Status: (U//FOUO) STUCCOMONTANA under development and is expected to be released by 30 November 2008.

[^0]
[^0]:    POC: U//FOUO
    S32222.
    2ensa.gov
![img-19.jpeg](img-19.jpeg)

CTX4000
ANT Product Data
(TS//SI//REL TO USA,FVEY) The CTX4000 is a portable continuous wave (CW) radar unit. It can be used to illuminate a target system to recover different off net information. Primary uses include VAGRANT and DROPMIRE collection.
![img-20.jpeg](img-20.jpeg)
(TS//SI//REL TO USA,FVEY) The CTX4000 provides the means to collect signals that otherwise would not be collectable, or would be extremely difficult to collect and process. It provides the following features:

- Frequency Range: 1 - 2 GHz .
- Bandwidth: Up to 45 MHz
- Output Power: User adjustable up to 2 W using the internal amplifier; external amplifiers make it possible to go up to 1 kW .
- Phase adjustment with front panel knob
- User-selectable high- and low-pass filters.
- Remote controllable
- Outputs:
- Transmit antenna
- I \& Q video outputs
- DC bias for an external pre-amp on the Receive input connector
- Inputs:
- External oscillator
- Receive antenna


# Unit Cost: N/A 

Status: unit is operational. However, it is reaching the end of its service life. It is scheduled to be replaced by PHOTOANGLO starting in September 2008.
![img-21.jpeg](img-21.jpeg)
![img-22.jpeg](img-22.jpeg)

# LOUDAUTO ANT Product Data 

(TSI/SI/IREL TO USA,FVEY) Audio-based RF retro-reflector. Provides room audio from targeted space using radar and basic post-processing.

## (U) Capabilities

(TSI/SI/IREL TO USA,FVEY) LOUDAUTO's current design maximizes the gain of the microphone. This makes it extremely useful for picking up room audio. It can pick up speech at a standard, office volume from over 20' away. (NOTE: Concealmente may reduce this distance.) It uses very little power ( $\sim 15 \mathrm{uA}$ at 3.0 VDC ), so little, in fact, that battery self-discharge is more of an issue for serviceable lifetime than the power draw from this unit. The simplicity of the design allows the form factor to be tailored for specific operational requirements. All components at
![img-23.jpeg](img-23.jpeg)

COTS and so are non-attributable to NSA.

## (U) Concept of Operation

TSI/SI/IREL TO USA,FVEY) Room audio is picked up by the microphone and converted into an analog electrical signal. This signal is used to pulse position modulate (PPM) a square wave signal running at a pre-set frequency. This square wave is used to turn a FET (field effect transistor) on and off. When the unit is illuminated with a CW signal from a nearby radar unit, the illuminating signal is amplitude-modulated with the PPM square wave. This signal is re-radiated, where it is picked up by the radar, then processed to recover the room audio. Processing is currently performed by COTS equipment with FM demodulation capability (Rohde \& Schwarz FSH-series portable spectrum analyzers, etc.) LOUDAUTO is part of the ANGRYNEIGHBOR family of radar retro-reflectors.

Unit Cost: $\$ 30$
Status: End processing still in development
POC:
S32243, $\square$
![img-24.jpeg](img-24.jpeg)

# NIGHTSTAND 

## Wireless Exploitation / Injection Tool

(TSI/SI/IREL) An active 802.11 wireless exploitation and injection tool for payload/exploit delivery into otherwise denied target space. NIGHTSTAND is typically used in operations where wired access to the target is not possible.
(TSI/SI//REL) NIGHTSTAND - Close Access Operations $\cdot$ Battlefield Tested - Windows Exploitation $\cdot$ Standalone System

## System Details

$>$ (U//FOUO) Standalone tool currently running on an x86 laptop loaded with Linux Fedora Core 3.
$>$ (TSI/SI//REL) Exploitable Targets include Win2k, WinXP, WinXPSP1, WINXPSP2 running internet Explorer versions 5.0-6.0.
$>$ (TSI/SI//REL) NS packet injection can target one client or multiple targets on a wireless network.
$>$ (TSI/SI//REL) Attack is undetectable by the user.
![img-25.jpeg](img-25.jpeg)

NIGHTSTAND Hardware
(TSI/SI/IREL) Use of external amplifiers and antennas in both experimental and operational scenarios have resulted in successful NIGHTSTAND attacks from as far away as eight miles under ideal environmental conditions.

Unit Cost: Varies from platform to platform
Status: Product has been deployed in the field. Upgrades to the system continue to be developed.

POC: $\square$ S32242, $\square$
![img-26.jpeg](img-26.jpeg)

# NIGHTWATCH ANT Product Data 

(TS//SI//REL TO USA,FVEY) NIGHTWATCH is a portable computer with specialized, internal hardware designed to process progressive-scan (noninterlaced) VAGRANT signals.

## (U) Capability Summary

(TS//SI//REL TO USA,FVEY) The current implementation of NIGHTWATCH consists of a general-purpose PC inside of a shielded case. The PC has PCI digitizing and clock cards to provide the needed interface and accurate clocking required for video reconstruction. It also has:

- horizontal sync, vertical sync and video outputs to drive an external, multi-sync monitor.
- video input
- spectral analysis up to 150 kHz to provide for indications of horizontal and vertical sync frequencies
- frame capture and forwarding
- PCMCIA cards for program and data storage
- horizontal sync locking to keep the display set on the NIGHTWATCH display.
- frame averaging up to $2^{\wedge} 16$ (65536) frames.


## (U) Concept of Operation

(TS//SI//REL TO USA,FVEY) The video output from an appropriate collection system, such as a CTX4000, PHOTOANGLO, or general-purpose receiver, is connected to the video input on the NIGHTWATCH system. The user, using the appropriate tools either within NIGHTWATCH or externally, determines the horizontal and vertical sync frequencies of the targeted monitor. Once the user matches the proper frequencies, he activates "Sync Lock" and frame averaging to reduce noise and improve readability of the targeted monitor. If warranted, the user then forwards the displayed frames over a network to NSAW, where analysts can look at them for intelligence purposes.

## Unit Cost: N/A

Status: This system has reached the end of its service life. All work concerning the NIGHTWATCH system is strictly for maintenance purposes. This system is slated to be replaced by the VIEWPLATE system.
![img-27.jpeg](img-27.jpeg)
![img-28.jpeg](img-28.jpeg)

# PHOTOANGLO ANT Product Data 

(TSI/SI/IREL TO USA,FVEY) PHOTOANGLO is a joint NSA/GCHQ project to develop a new radar system to take the place of the CTX4000.

24 Jul 2008

## (U) Capabilities

(TSI/SI/IREL TO USA,FVEY) The planned capabilities for this system are: -Frequency range: $1-2 \mathrm{GHz}$, which will be later extended to $1-4 \mathrm{GHz}$.
-Maximum bandwidth: 450 MHz .
-Size: Small enough to fit into a slim briefcase.
$\bullet$ Weight: Less than 10 lbs.
-Maximum Output Power: 2 W
-Output:
-Video
-Transmit antenna
$\bullet$ Inputs:
-External oscillator
-Receive antenna

## (U) Concept of Operation

(TSI/SI/IREL TO USA,FVEY) TS//SI//REL TO USA,FVEY) The radar unit generates an un-modulated, continuous wave (CW) signal. The oscillator is either generated internally, or externally through a signal generator or cavity oscillator. The unit amplifies the signal and sends it out to an RF connector, where it is directed to some form of transmission antenna (horn, parabolic dish, LPA, spiral). The signal illuminates the target system and is re-radiated. The receive antenna picks up the re-radiated signal and directs the signal to the receive input. The signal is amplified, filtered, and mixed with the transmit antenna. The result is a homodyne receiver in which the RF signal is mixed directly to baseband. The baseband video signal is ported to an external BNC connector. This connects to a processing system, such as NIGHTWATCH, an LFS-2, or VIEWPLATE, to process the signal and provide the intelligence.

Unit Cost: $\$ 40 \mathrm{k}$ (planned)
Status: Development. Planned IOC is 1st QTR FY09.
POC: S32243, $\square$
![img-29.jpeg](img-29.jpeg)

# SPARROW II 

Wireless Survey - Airborne Operations - UAV
(TSI/SI/IREL) An embedded computer system running BLINDDATE tools. Sparrow II is a fully functional WLAN collection system with integrated Mini PCI slots for added functionality such as GPS and multiple Wireless Network Interface Cards.

## (UI/FOUO) System Specs

Processor: IBM Power PC 405GPR Memory: 64MB (SDRAM) 16 MB (FLASH)

Expansion: Mini PCI (Up to 4 devices) supports USB, Compact Flash, and 802.11 B/G

OS: Linux (2.4 Kernel)
![img-30.jpeg](img-30.jpeg)

SPARROW II Hardware

Application SW: BLINDDATE
Battery Time: At least two hours
(TSI/SI/IREL) The Sparrow II is a capable option for deployment where small size, minimal weight and reduced power consumption are required. PCI devices can be connected to the Sparrow II to provide additional functionality, such as wireless command and control or a second or third 802.11 card. The Sparrow II is shipped with Linux and runs the BLINDDATE software suite.

Unit Cost: $\$ 6 \mathrm{~K}$
Status: (S//SI//REL) Operational Restrictions exist for equipment deployment.
POC: S32242,
![img-31.jpeg](img-31.jpeg)

# TAWDRYYARD ANT Product Data 

(TS//SI//REL TO USA,FVEY) Beacon RF retro-reflector. Provides return when illuminated with radar to provide rough positional location.

## (U) Capabilities

(TS//SI//REL TO USA,FVEY) TAWDRYYARD is used as a beacon, typically to assist in locating and identifying deployed RAGEMASTER units. Current design allows it to be detected and located quite easily within a $50^{\prime}$ radius of the radar system being used to illuminate it. TAWDRYYARD draws as $8 \mu \mathrm{~A}$ at $2.5 \mathrm{~V}(20 \mu \mathrm{~W})$ allowing a standard lithium coin cell to power it for months or years. The simplicity of the design allows the form factor to be tailored for specific operational requirements. Future capabilities being considered are return of GPS coordinates and a unique target identifier and automatic processing to scan a target area for presence of TAWDRYYARDs. All components are COTS and so are non-attributable to NSA.

## (U) Concept of Operation

(TS//SI//REL TO USA,FVEY) The board generates a square wave operating at a preset frequency. This square wave is used to turn a FET (field effect transistor) on and off. When the unit is illuminated with a CW signal, the illuminating signal is amplitude-modulated (AM) with the square wave. This signal is re-radiated, where it is picked up by the radar, then processed to recover the clock signal. Typically, the fundamental is used to indicate the unit's presence, and is simply displayed on a low frequency spectrum analyzer. TAWDRYYARD is part of the ANGRYNEIGHBOR family of radar retro-reflectors.

Unit Cost: $\$ 30$
Status: End processing still in development
POC: S32243, fênsa.ic.gov
![img-32.jpeg](img-32.jpeg)

# GINSU <br> ANT Product Data 

(TSI/SII/REL) GINSU provides software application persistence for the CNE implant, KONGUR, on target systems with the PCI bus hardware implant, BULLDOZER.
![img-33.jpeg](img-33.jpeg)
(TSI/SI/REL) GINSU Extended Concept of Operations
(TSI/SI/REL) This technique supports any desktop PC system that contains at least one PCI connector (for BULLDOZER installation) and Microsoft Windows 9x, 2000, 2003, XP, or Vista.
(TSI/SI//REL) Through interdiction, BULLDOZER is installed in the target system as a PCI bus hardware implant. After fielding, if KONGUR is removed from the system as a result of an operating system upgrade or reinstall, GINSU can be set to trigger on the next reboot of the system to restore the software implant.

Status: Released / Deployed. Ready for Immediate Delivery

Unit Cost: $\$ 0$
![img-34.jpeg](img-34.jpeg)
![img-35.jpeg](img-35.jpeg)

# HOWLERMONKEY ANT Product Data 

(TSI/SII/REL) HOWLERMONKEY is a custom Short to Medium Range Implant RF Transceiver. It is used in conjunction with a digital core to provide a complete implant.

HOWLERMONKEY -
SUTURESAILOR
![img-36.jpeg](img-36.jpeg)
$1.23^{\prime \prime}(31.25 \mathrm{~mm})$
$\times 0.48^{\prime \prime}(12.2 \mathrm{~mm})$
HOWLERMONKEY -
SUTURESAILOR
![img-37.jpeg](img-37.jpeg)
$1.20^{\prime \prime}(30.5 \mathrm{~mm})$
$\times 0.23^{\prime \prime}(6 \mathrm{~mm})$

HOWLERMONKEY - YELLOWPIN
![img-38.jpeg](img-38.jpeg)
$2^{\prime \prime}(50.8 \mathrm{~mm}) \times 0.45^{\prime \prime}(11.5 \mathrm{~mm})$
(Actual Size)
![img-39.jpeg](img-39.jpeg)
$0.63^{\prime \prime}(16 \mathrm{~mm}) \times$
$0.63^{\prime \prime}(16 \mathrm{~mm})$

## HOWLERMONKEY

FIREWALK
![img-40.jpeg](img-40.jpeg)
$0.63^{\prime \prime}(16 \mathrm{~mm})$

## (TSI/SII/REL) HOWLERMONKEY is a COTS-based transceiver designed to be compatible with CONJECTURE/SPECULATION networks and STRIKEZONE devices running a HOWLERMONKEY personality. PCB layouts are tailored to individual implant space requirements and can vary greatly in form factor.

Implant 1
![img-41.jpeg](img-41.jpeg)

Implant 2
![img-42.jpeg](img-42.jpeg)

## 40 units: \$750/ each

25 units: $\$ 1,000 /$ each

## HOWLERMONKEY

Transceiver

## 25 units: $\$ 1,000 /$ each

![img-43.jpeg](img-43.jpeg)
![img-44.jpeg](img-44.jpeg)

# IRATEMONK 

## ANT Product Data

(TS//SI//REL) IRATEMONK provides software application persistence on desktop and laptop computers by implanting the hard drive firmware to gain execution through Master Boot Record (MBR) substitution.
![img-45.jpeg](img-45.jpeg)
(TSI/SI//REL) IRATEMONK Extended Concept of Operations
(TSI/SI//REL) This technique supports systems without RAID hardware that boot from a variety of Western Digital, Seagate, Maxtor, and Samsung hard drives. The supported file systems are: FAT, NTFS, EXT3 and UFS.
(TSI/SI//REL) Through remote access or interdiction, UNITEDRAKE, or STRAITBAZZARE are used in conjunction with SLICKERVICAR to upload the hard drive firmware onto the target machine to implant IRATEMONK and its payload (the implant installer). Once implanted, IRATEMONK's frequency of execution (dropping the payload) is configurable and will occur when the target machine powers on.

Status: Released / Deployed. Ready for
Unit Cost: $\$ 0$ Immediate Delivery
![img-46.jpeg](img-46.jpeg)

# JUNIORMINT ANT Product Data 

(TSI/SII/REL) JUNIORMINT is a digital core packaged in both a mini Printed Circuit Board (PCB), to be used in typical concealments, and a miniaturized Flip Chip Module (FCM), to be used in implants with size constraining concealments.
(TSI/SII/REL) JUNIORMINT uses the TAO standard implant architecture. The architecture provides a robust, reconfigurable, standard digital platform resulting in a dramatic performance improvement over the obsolete HC12 microcontroller based designs. A mini Printed Circuit Board (PCB) using packaged parts will be developed and will be available as the standard platform for applications requiring a digital core. The ultra-miniature Flip Chip Module (FCM) will be available for challenging concealments. Both will contain an ARM9 microcontroller, FPGA, Flash, SDRAM and DDR2 memories.

| uController | Flash | SDRAM | FPGA | DDR2 |
| :--: | :--: | :--: | :--: | :--: |
| ARM 9 <br> 400 MHz | 32 MBytes | MT48H16M32LF <br> 64 MBytes | XC4VLX25 <br> 10752 Slice | MT47H64M16 <br> 128 MBytes |

![img-47.jpeg](img-47.jpeg)
TOP SECRET//COMINT//REL TO USA, FVEY
![img-48.jpeg](img-48.jpeg)

# MAESTRO-II <br> ANT Product Data 

(TSI/SII/REL) MAESTRO-II is a miniaturized digital core packaged in a Multi-Chip Module (MCM) to be used in implants with size constraining concealments.
![img-49.jpeg](img-49.jpeg)

Status: Available - On The Shelf
![img-50.jpeg](img-50.jpeg)

Derived From: NSACSSM 1-52
Dated: 20070108
Declassify On: 20320108
![img-51.jpeg](img-51.jpeg)

# SOMBERKNAVE ANT Product Data 

(TSI/SII/REL) SOMBERKNAVE is Windows XP wireless software implant that provides covert internet connectivity for isolated targets.
(TSI/SII/REL) SOMBERKNAVE is a software implant that surreptitiously routes TCP traffic from a designated process to a secondary network via an unused embedded 802.11 network device. If an Internet-connected wireless Access Point is present, SOMBERKNAVE can be used to allow OLYMPUS or VALIDATOR to "call home" via 802.11 from an air-gapped target computer. If the 802.11 interface is in use by the target, SOMBERKNAVE will not attempt to transmit.
(TSI/SII/REL) Operationally, VALIDATOR initiates a call home. SOMBERKNAVE triggers from the named event and tries to associate with an access point. If connection is successful, data is sent over 802.11 to the ROC. VALIDATOR receives instructions, downloads OLYMPUS, then disassociates and gives up control of the 802.11 hardware. OLYMPUS will then be able to communicate with the ROC via SOMBERKNAVE, as long as there is an available access point.
![img-52.jpeg](img-52.jpeg)

Status: Available - Fall 2008
Unit Cost: $\$ 50 \mathrm{k}$
![img-53.jpeg](img-53.jpeg)
![img-54.jpeg](img-54.jpeg)

# SWAP 

## ANT Product Data

(TSI/SI/IREL) SWAP provides software application persistence by exploiting the motherboard BIOS and the hard drive's Host Protected Area to gain periodic execution before the Operating System loads.
![img-55.jpeg](img-55.jpeg)
(TSI/SI/IREL) SWAP Extended Concept of Operations
(TSI/SI/IREL) This technique supports single or multi-processor systems running Windows, Linux, FreeBSD, or Solaris with the following file systems: FAT32, NTFS, EXT2, EXT3, or UFS 1.0.
(TSI/SI/IREL) Through remote access or interdiction, ARKSTREAM is used to reflash the BIOS and TWISTEDKILT to write the Host Protected Area on the hard drive on a target machine in order to implant SWAP and its payload (the implant installer). Once implanted, SWAP's frequency of execution (dropping the payload) is configurable and will occur when the target machine powers on.

Status: Released / Deployed. Ready for
Unit Cost: $\$ 0$ Immediate Delivery
![img-56.jpeg](img-56.jpeg)

# TRINITY ANT Product Data 

(TSI/SII/REL) TRINITY is a miniaturized digital core packaged in a Multi-Chip Module (MCM) to be used in implants with size constraining concealments.
![img-57.jpeg](img-57.jpeg)
(TSI/SII/REL) TRINITY uses the TAO standard implant architecture. The architecture provides a robust, reconfigurable, standard digital platform resulting in a dramatic performance improvement over the obsolete HC12 microcontroller based designs. A development Printed Circuit Board (PCB) using packaged parts has been developed and is available as the standard platform. The TRINITY Multi-Chip-Module (MCM) contains an ARM9 microcontroller, FPGA, Flash and SDRAM memories.

| uController | Flash | SDRAM (3) | FPGA |
| :--: | :--: | :--: | :--: |
| ARM 9 | AT49BV322A | MT48LC8M32 | XC2V1000 |
| 180 Mhz | 4 MBytes | 96 MBytes | 1M gates |

![img-58.jpeg](img-58.jpeg)

Status: Special Order due vendor selected.
Unit Cost: 100 units: $\$ 625 \mathrm{~K}$
POC: S3223, S3223, S3223,
![img-59.jpeg](img-59.jpeg)
![img-60.jpeg](img-60.jpeg)

# SURLYSPAWN <br> ANT Product Data 

(TS//SI//REL TO USA,FVEY) Data RF retro-reflector. Provides return modulated with target data (keyboard, low data rate digital device) when illuminated with radar.

## (U) Capabilities

(TS//SI//REL TO USA,FVEY) SURLYSPAWN has the capability to gather keystrokes without requiring any software running on the targeted system. It also only requires that the targeted system be touched once. The retro-reflector is compatible with both USB and PS/2 keyboards. The simplicity of the design allows the form factor to be tailored for specific operational requirements. Future capabilities will include laptop keyboards.

## (U) Concept of Operation

![img-61.jpeg](img-61.jpeg)
(TS//SI//REL TO USA,FVEY) The board taps into the data line from the keyboard to the processor. The board generates a square wave oscillating at a preset frequency. The data-line signal is used to shift the square wave frequency higher or lower, depending on the level of the data-line signal. The square wave, in essence, becomes frequency shift keyed (FSK). When the unit is illuminated by a CW signal from a nearby radar, the illuminating signal is amplitude-modulated (AM) with this square wave. The signal is re-radiated, where it is received by the radar, demodulated, and the demodulated signal is processed to recover the keystrokes. SURLYSPAWN is part of the ANGRYNEIGHBOR family of radar retro-reflectors.

Unit Cost: $\$ 30$
Status: End processing still in development
POC: S32243, $\square$
![img-62.jpeg](img-62.jpeg)

# DROPOUTJEEP ANT Product Data 

(TSI/SI/IREL) DROPOUTJEEP is a STRAITBIZARRE based software implant for the Apple iPhone operating system and uses the CHIMNEYPOOL framework. DROPOUTJEEP is compliant with the FREEFLOW project, therefore it is supported in the TURBULENCE architecture.
![img-63.jpeg](img-63.jpeg)
(U/FOUO) DROPOUTJEEP - Operational Schematic
(TSI/SI/IREL) DROPOUTJEEP is a software implant for the Apple iPhone that utilizes modular mission applications to provide specific SIGINT functionality. This functionality includes the ability to remotely push/pull files from the device, SMS retrieval, contact list retrieval, voicemail, geolocation, hot mic, camera capture, cell tower location, etc. Command, control, and data exfiltration can occur over SMS messaging or a GPRS data connection. All communications with the implant will be covert and encrypted.
(TSI/SI/IREL) The initial release of DROPOUTJEEP will focus on installing the implant via close access methods. A remote installation capability will be pursued for a future release.

Unit Cost: $\$ 0$
Status: (U) In development
POC: U//FOUO
S32222.
iPensa.gov
![img-64.jpeg](img-64.jpeg)

# GOPHERSET ANT Product Data 

(TSI/SII/REL) GOPHERSET is a software implant for GSM (Global System for Mobile communication) subscriber identify module (SIM) cards. This implant pulls Phonebook, SMS, and call log information from a target handset and exfiltrates it to a user-defined phone number via short message service (SMS).
![img-65.jpeg](img-65.jpeg)
(U//FOUO) GOPHERSET - Operational Schematic
(TSI/SI/REL) Modern SIM cards (Phase 2+) have an application program interface known as the SIM Toolkit (STK). The STK has a suite of proactive commands that allow the SIM card to issue commands and make requests to the handset. GOPHERSET uses STK commands to retrieve the requested information and to exfiltrate data via SMS. After the GOPHERSET file is compiled, the program is loaded onto the SIM card using either a Universal Serial Bus (USB) smartcard reader or via over-the-air provisioning. In both cases, keys to the card may be required to install the application depending on the service provider's security configuration.

Unit Cost: $\$ 0$
Status: (U//FOUO) Released. Has not been deployed.
POC: U//FOUO
S32222.
Tênsa.gov
![img-66.jpeg](img-66.jpeg)

# MONKEYCALENDAR ANT Product Data 

(TSI/SI//REL) MONKEYCALENDAR is a software implant for GSM (Global System for Mobile communication) subscriber identify module (SIM) cards. This implant pulls geolocation information from a target handset and exfiltrates it to a userdefined phone number via short message service (SMS).
![img-67.jpeg](img-67.jpeg)
(US//SO//REL) Modern SIM cards (Phase 2+) have an application program interface known as the SIM Toolkit (STK). The STK has a suite of proactive commands that allow the SIM card to issue commands and make requests to the handset. MONKEYCALENDAR uses STK commands to retrieve location information and to exfiltrate data via SMS. After the MONKEYCALENDAR file is compiled, the program is loaded onto the SIM card using either a Universal Serial Bus (USB) smartcard reader or via over-the-air provisioning. In both cases, keys to the card may be required to install the application depending on the service provider's security configuration

## Unit Cost: $\$ 0$

Status: Released, not deployed.
POC: U//FOUO
S32222
Tênsa.gov
![img-68.jpeg](img-68.jpeg)

# PICASSO 

GSM HANDSET
(SI/SI/IREL) Modified GSM (target) handset that collects user data, location information and room audio. Command and data exfil is done from a laptop and regular phone via SMS - (Short Messaging Service), without alerting the target.
(S/ISI) Target Data via SMS:

- Incoming call numbers
- Outgoing call numbers
- Recently registered networks
- Recent Location Area Codes (LAC)
- Cell power and Timing Advance information (GEO)
- Recently Assigned TMSI, IMSI
- Recent network authentication
challenge responses
- Recent successful PINs entered into the phone during the power-on cycle -SW version of PICASSO implant
- Hot-mic' to collect Room Audio
- Panic Button sequence (sends location information to an LP Operator)
- Send Targeting Information (i.e.
current IMSI and phone number when it is turned on - in case the SIM has just been switched).
-Block call to deny target service.
(S/ISI) PICASSO Operational Concept
(SI/SI/IREL) Uses include asset validation and tracking and target templating. Phone can be hot mic'd and has a "Panic Button" key sequence for the witting user.

Status: 2 weeks ARO (10 or less)
(S/ISI/IREL) Handset
Options
-Eastcom 760c+
-Samsung E600, X450
-Samsung C140
-(with Arabic keypad/language option)
![img-69.jpeg](img-69.jpeg)

Unit Cost: approx \$2000
![img-70.jpeg](img-70.jpeg)

Derived From: NSA/CSSM 1-52
Dated: 20070108
Declassify On: 20320108
![img-71.jpeg](img-71.jpeg)

# TOTECHASER ANT Product Data 

(TSI/SI/IREL) TOTECHASER is a Windows CE implant targeting the Thuraya 2520 handset. The Thuraya 2520 is a dual mode phone that can operate either in SAT or GSM modes. The phone also supports a GPRS data connection for Web browsing, e-mail, and MMS messages. The initial software implant capabilities include providing GPS and GSM geo-location information. Call log, contact list, and other user information can also be retrieved from the phone. Additional capabilities are being investigated.
![img-72.jpeg](img-72.jpeg)
(US/ISI/IREL) TOTECHASER will use SMS messaging for the command, control, and data exfiltration path. The initial capability will use covert SMS messages to communicate with the handset. These covert messages can be transmitted in either Thuraya Satellite mode or GSM mode and will not alert the user of this activity. An alternate command and control channel using the GPRS data connection based on the TOTEGHOSTLY implant is intended for a future version.
(TSI/SI/IREL) Prior to deployment, the TOTECHASER handsets must be modified. Details of how the phone is modified are being developed. A remotely deployable TOTECHASER implant is being investigated. The TOTECHASER system consists of the modified target handsets and a collection system.
(TSI/SI/IREL) TOTECHASER will accept configuration parameters to determine how the implant operates. Configuration parameters will determine what information is recorded, when to collect that information, and when the information is exfiltrated. The configuration parameters can be set upon initial deployment and updated remotely.

## Unit Cost: $\$$

## Status:

POC: U/FOUO, S32222, $\qquad$ Eensa.gov

Derived From: NSA/CSSM 1-52
Dated: 20070108
Declassify On: 20320108
TOP SECRET//COMINT//REL TO USA, FVEY
![img-73.jpeg](img-73.jpeg)

# TOTEGHOSTLY 2.0 <br> ANT Product Data 

(TS//SI//REL) TOTEGHOSTLY 2.0 is a STRAITBIZARRE based implant for the Windows Mobile embedded operating system and uses the CHIMNEYPOOL framework. TOTEGHOSTLY 2.0 is compliant with the FREEFLOW project, therefore it is supported in the TURBULENCE architecture.
![img-74.jpeg](img-74.jpeg)
(U//FOUO) TOTEGHOSTLY - Data Flow Schematic
(TS//SI//REL) TOTEGHOSTLY 2.0 is a software implant for the Windows Mobile operating system that utilizes modular mission applications to provide specific SIGINT functionality. This functionality includes the ability to remotely push/pull files from the device, SMS retrieval, contact list retrieval, voicemail, geolocation, hot mic, camera capture, cell tower location, etc. Command, control, and data exfiltration can occur over SMS messaging or a GPRS data connection. A FRIEZERAMP interface using HTTPSlink2 transport module handles encrypted communications.
(TS//SI//REL) The initial release of TOTEGHOSTLY 2.0 will focus on installing the implant via close access methods. A remote installation capability will be pursued for a future release.
(TS//SI//REL) TOTEGHOSTLY 2.0 will be controlled using an interface tasked through the NCC (Network Control Center) utilizing the XML based tasking and data forward scheme under the TURBULENCE architecture following the TAO GENIE Initiative.

Unit Cost: $\$ 0$
Status: (U) In development
POC: U//FOUO
S32222, $\square$ fensa.gov
Derived From: NSA/CSSM 1-52
Dated: 20070108
Declassify On: 20320108
![img-75.jpeg](img-75.jpeg)

# CANDYGRAM GSM Telephone Tripwire 

(S//SI//REL) Mimics GSM cell tower of a target network. Capable of operations at 900, 1800, or 1900 MHz . Whenever a target handset enters the CANDYGRAM base station's area of influence, the system sends out an SMS through the external network to registered watch phones.
![img-76.jpeg](img-76.jpeg)
(SI/SI//REL) CANDYGRAM Operational Concept
(SI/SI//REL) Typical use scenarios are asset validation, target tracking and identification as well as identifying hostile surveillance units with GSM handsets. Functionality is predicated on apriori target information.

## (S//SI//REL) System HW

- GPS processing unit
- Tri-band BTS radio
- Windows XP laptop and cell phone*
-9" wide x 12 " long x 2 " deep
- External power (9-30 VDC).
*Remote control software can be used with any connected to the laptop (used for communicating with the CANDYGRAM unit through text messages (SMS).


## (S//SI//REL) SW Features

- Configurable 200 phone number target deck.
- Network auto-configuration
- Area Survey Capability
- Remote Operation Capability
- Configurable Network emulation
- Configurable RF power level
- Mutli-Units under single C\&C
- Remote restart
- Remote erasure (not field recoverable)

Status: Available 8 mos ARO
Unit Cost: approx \$40K
![img-77.jpeg](img-77.jpeg)

# CROSSBEAM 

## ANT Product Data

(TS//SI//REL) CROSSBEAM is a GSM module that mates a modified commercial cellular product with a WAGONBED controller board.
![img-78.jpeg](img-78.jpeg)
![img-79.jpeg](img-79.jpeg)

# CYCLONE Hx9 

## Base Station Router

(SI/SII/FVEY) EGSM (900MGz) macro-class Network-In-a-Box (NIB) system. Uses the existing Typhon GUI and supports the full Typhon feature base and applications.
(SI/SII/REL) Operational Restrictions exist for equipment deployment.
![img-80.jpeg](img-80.jpeg)
$>$ (S//SI//REL) Features:

- EGSM 900MHz
-Macro-class (+43dBm)
- 32+Km Range
- Optional Battery Kits
- Highly Mobile and Deployable
- Integrated GPS, MS, \& 802.11
- Voice \& High-speed Data
- GSM Security \& Encryption
$>$ (S//SI//REL) Advanced Features:
- GPS - Supporting Typhon applications
- GSM Handset Module - Supports auto-configuration and remote command and control features.
- 802.11 - Supports high speed wireless LAN remote command and control
( SIISI/REL) Enclosure:
- $3.5^{\circ} \mathrm{H} \times 8.5^{\circ} \mathrm{W} \times 9^{\circ} \mathrm{D}$
- Approximately 8 lbs
- Actively cooled for extreme environments
$>$ (S//SI//REL) Cyclone Hx9 System Kit:
- Cyclone Hx9 System
- AC/DC power converter
- Antenna to support MS, GPS, WIFI, \& RF
- LAN, RF, \& USB cables
- Pelican Case
- (Field Kit only) Control Laptop and Accessories
$>$ (S//SI//REL) Separately Priced Options:
- 800 WH Lilon Battery Kit
$>$ (S//SI//REL) Base Station Router Platform:
- Overlay GSM cellular communications supporting up to 32 Cyclone Mx9 systems providing full mobility and utilizing a VoIP back-haul.
- GPRS data service and associated application

Unit Cost: $\$ 70 \mathrm{~K}$ for two months
Status: Just out of development, first production runs ongoing.
Derived From: NSA/CSSM 1-52
Dated: 20070108
Oecilassify On: 20320108
![img-81.jpeg](img-81.jpeg)

# Low Power GSM Active Interrogator 

(S//SI//REL) Multi-purpose, Pico class, tri-band active GSM base station with internal 802.11/GPS/handset capability.
(S//SI//REL) Operational Restrictions exist for equipment deployment.
![img-82.jpeg](img-82.jpeg)
$>$ (S//SI//REL) Features:

- LxT Model: 900/1800/1900MHz
- LxU Model: 850/1800/1900MHz
- Pico-class (1Watt) Base station
- Optional Battery Kits
- Highly Mobile and Deployable
- Integrated GPS, MS, \& 802.11
- Voice \& High-speed Data
- SMS Capability
$>$ (S//SI//REL) Enclosure:
- $1.9^{\circ} \mathrm{H} \times 8.6^{\circ} \mathrm{W} \times 6.3^{\circ} \mathrm{D}$
- Approximately 3 lbs
- Actively cooled for extreme environments
$>$ (S//SI//REL) EBSR System Kit:
- EBSR System
- AC/DC power converter
- Antennas to support MS, GPS, WIFI, \& RF
- LAN, RF, \& USB cables
- Pelican Case
- (Field Kit only) Control Laptop and Accessories
$>$ (S//SI//REL) Separately Priced Options:
- 90 WH Lilon Battery Kit
$>$ (S//SI//REL) Base Station Router Platform:
- Multiple BSR units can be interconnected to form a macro network using 802.3 and 802.11 back-haul.
- Supports Landshark/Candygram capabilities.

Status:
Unit Cost: $\$ 40 \mathrm{~K}$

POC: $\square$ S32242, $\square$
![img-83.jpeg](img-83.jpeg)

# ENTOURAGE <br> (S//SI//REL) Direction Finding on HollowPoint Platform 

(S//SI//REL) Direction Finding application operating on the HOLLOWPOINT platform. The system is capable of providing line of bearing for GSM/UMTS/ CDMA2000/FRS signals. A band-specific antenna and laptop controller is needed to compliment the HOLLOWPOINT system and completes the ground based system.
![img-84.jpeg](img-84.jpeg)
(S//SI//REL) HOLLOWPOINT SDR Platform and Antenna
(S//SI) The ENTOURAGE application leverages the 4 Software Defined Radio (SDR) units in the HOLLOWPOINT platform. This capability provides an "Artemislike" capability for waveforms of interest (2G,3G, others). The ENTOURAGE application works in conjunction with the NEBULA active interrogator as part of the Find/Fix/Finish capabilities of the GALAXY program.
$>$ (S//SI//REL) Features:

- Software Defined Radio System
- Operating range $10 \mathrm{MHz}-4 \mathrm{GHz}$
- 4 Receive paths, all synchronized
- 1 Transmit path
- DF capability on

GSM/UMTS/CDMA2000/ FRS signals

- Gigabit Ethernet
- Integrated GPS
- Highly Mobile and Deployable

Status: The system is in the final testing stage and Unit Cost: $\$ 70 \mathrm{~K}$ will be in production Spring 09.

| $>$ (S//SI//REL) Enclosure: |  |
| :--: | :--: |
| - $1.8^{\circ} \mathrm{H} \times 8.0^{\circ} \mathrm{W} \times 8.0^{\circ} \mathrm{D}$ |  |
| - Approximately 3 lbs |  |
| - 15 Watts |  |
| - Passively cooled |  |
| $>$ (S//SI//REL) Future Developments: |  |
| - WiMAX |  |
| - WiFi |  |
| - LTE |  |
![img-85.jpeg](img-85.jpeg)

# GENESIS 

## Covert SIGINT Transceiver

(SI/SII/REL) Commercial GSM handset that has been modified to include a Software Defined Radio (SDR) and additional system memory. The internal SDR allows a witting user to covertly perform network surveys, record RF spectrum, or perform handset location in hostile environments.
(SI/SII/REL) GENESIS Handset
(SI/SII/REL) The GENESIS systems are designed to support covert operations in hostile environments. A witting user would be able to survey the local environment with the spectrum analyzer tool, select spectrum of interest to record, and download the spectrum information via the integrated Ethernet to a laptop controller. The GENESIS system could also be used, in conjunction with an active interrogator, as the finishing tool when performing Find/Fix/Finish operations in unconventional environments.
$>$ (S//SII/REL) Features:

- Concealed SDR with Handset Menu Interface
- Spectrum Analyzer Capability
- Find/Fix/Finish Capability
- Integrated Ethernet
- External Antenna Port
- Internal 16 GB of storage
- Multiple Integrated Antennas

Status: Current GENESIS platform available.
Future platforms available when developments are completed.
![img-86.jpeg](img-86.jpeg)

[^0]
[^0]:    POC: $\square$ S32242, $\square$ S32242S32242S32242S32242S32242
    Derived From: NSA/CSSM 1-52
    Dated: 20070108
    Declassify On: 20320108
![img-87.jpeg](img-87.jpeg)

# NEBULA 

## Base Station Router

(SI/SII/FVEY) Multi-Protocol macro-class Network-In-a-Box (NIB) system. Leverages the existing Typhon GUI and supports GSM, UMTS, CDMA2000 applications. LTE capability currently under development.
(SI/SII/REL) Operational Restrictions exist for equipment deployment.
![img-88.jpeg](img-88.jpeg)
$>$ (S//SI//REL) Features:

- Dual Carrier System
- EGSM 900MHz
- UMTS 2100MHz
- CDMA2000 1900MHz
- Macro-class Base station
- Optional Battery Kits
- Highly Mobile and Deployable
- Integrated GPS, MS, \& 802.11
- Voice \& High-speed Data
$>$ (S//SI//REL) Advanced Features:
- GPS - Supporting NEBULA applications
- Designed to be self-configuring with security and encryption features
- 802.11 - Supports high speed wireless LAN remote command and control

Status:
$>$ (S//SI//REL) Enclosure:

- $8.5^{\circ} \mathrm{H} \times 13.0^{\circ} \mathrm{W} \times 16.5^{\circ} \mathrm{D}$
- Approximately 45 lbs
- Actively cooled for extreme environments
$>$ (S//SI//REL) NEBULA System Kit:
- NEBULA System
- 3 Interchangeable RF bands
- AC/DC power converter
- Antenna to support MS, GPS, WIFI, \& RF
- LAN, RF, \& USB cables
- Pelican Case
- (Field Kit only) Control Laptop and Accessories
$>$ (S//SI//REL) Separately Priced Options:
- 1500 WH Lilon Battery Kit
$>$ (S//SI//REL) Base Station Router Platform:
- Multiple BSR units can be interconnected to form a macro network using 802.3 and 802.11 back-haul.
- Future GPRS and HSDPA data service and associated applications
![img-89.jpeg](img-89.jpeg)

# TYPHON HX 

## GSM Base Station Router

(SI/SII/FVEY) Base Station Router - Network-In-a-Box (NIB) supporting GSM bands 850/900/1800/1900 and associated full GSM signaling and call control.
![img-90.jpeg](img-90.jpeg)
![img-91.jpeg](img-91.jpeg)

# WATERWITCH 

## Handheld Finishing Tool

(SI/SI) Hand held finishing tool used for geolocating targeted handsets in the field.

## (S//SI) Features:

- Split display/controller for flexible deployment capability
- External antenna for DFing target; internal antenna for communication with active interrogator
$\bullet$ Multiple technology capability based on SDR
![img-92.jpeg](img-92.jpeg)
(SI/SI) WATERWITCH Handset DF Set
Platform; currently UMTS, with GSM and CDMA2000 under development
- Approximate size 3" $\times 7.5^{\prime \prime} \times 1.25^{\prime \prime}$ (radio), $2.5^{\prime \prime} \times 5^{\prime \prime} \times 0.75^{\prime \prime}$ (display); radio shrink in planning stages
- Display uses E-Ink technology for low light emissions
(SI/SI) Tactical Operators use WATERWITCH to locate handsets (last mile) where handset is connected to Typhon or similar equipment interrogator. WATERWITCH emits tone and gives signal strength of target handset. Directional antenna on unit allows operator to locate specific handset.

[^0]
[^0]:    Status: Under Development. Available FY-2008 Unit Cost:
    LRIP Production due August 2008
    POC: $\square$ S32242, $\square$
![img-93.jpeg](img-93.jpeg)

# COTTONMOUTH-I 

## ANT Product Data

(TSI/SII/REL) COTTONMOUTH-I (CM-I) is a Universal Serial Bus (USB) hardware implant which will provide a wireless bridge into a target network as well as the ability to load exploit software onto target PCs.

## COTTONMOUTH - 1

![img-94.jpeg](img-94.jpeg)
(TSI/SII/REL) CM-I will provide air-gap bridging, software persistence capability, "in-field" reprogrammability, and covert communications with a host software implant over the USB. The RF link will enable command and data infiltration and exfiltration. CM-I will also communicate with Data Network Technologies (DNT) software (STRAITBIZARRE) through a covert channel implemented on the USB, using this communication channel to pass commands and data between hardware and software implants. CM-I will be a GENIE-compliant implant based on CHIMNEYPOOL.
(TSI/SII/REL) CM-I conceals digital components (TRINITY), USB 1.1 FS hub, switches, and HOWLERMONKEY (HM) RF Transceiver within the USB Series-A cable connector. MOCCASIN is the version permanently connected to a USB keyboard. Another version can be made with an unmodified USB connector at the other end. CM-I has the ability to communicate to other CM devices over the RF link using an over-the-air protocol called SPECULATION.

COTTONMOUTH CONOP
INTERNET Scenario
![img-95.jpeg](img-95.jpeg)

Status: Availability - January 2009
Unit Cost: 50 units: $\$ 1,015 \mathrm{~K}$
POC: S3223, S3223, S3223, S3223, S3223, S3223,
![img-96.jpeg](img-96.jpeg)

# COTTONMOUTH-II 

## ANT Product Data

(TSI/StI/REL) COTTONMOUTH-II (CM-II) is a Universal Serial Bus (USB) hardware Host Tap, which will provide a covert link over USB link into a targets network. CM-II is intended to be operate with a long haul relay subsystem, which is co-located within the target equipment. Further integration is needed to turn this capability into a deployable system.
![img-97.jpeg](img-97.jpeg)
(TSI/StI/REL) CM-II will provide software persistence capability, "in-field" re-programmability, and covert communications with a host software implant over the USB. CM-II will also communicate with Data Network Technologies (DNT) software (STRAITBIZARRE) through a covert channel implemented on the USB, using this communication channel to pass commands and data between hardware and software implants. CM-II will be a GENIEcompliant implant based on CHIMNEYPOOL.
(TSI/StI/REL) CM-II consists of the CM-I digital hardware and the long haul relay concealed somewhere within the target chassis. A USB 2.0 HS hub with switches is concealed in a dual stacked USB connector, and the two parts are hard-wired, providing a intra-chassis link. The long haul relay provides the wireless bridge into the target's network.

COTTONMOUTH - II (CM-II) CONOP
ANT Covert Network Scenario
![img-98.jpeg](img-98.jpeg)

## TOP SECRET//COMINT//REL TO USA, FVEY
![img-99.jpeg](img-99.jpeg)

# COTTONMOUTH-III <br> ANT Product Data 

(TSI/SII/REL) COTTONMOUTH-I (CM-I) is a Universal Serial Bus (USB) hardware implant, which will provide a wireless bridge into a target network as well as the ability to load exploit software onto target PCs.
![img-100.jpeg](img-100.jpeg)
(TSI/SII/REL) CM-III will provide air-gap bridging, software persistence capability, "in-field" re-programmability, and covert communications with a host software implant over the USB. The RF link will enable command and data infiltration and exfiltration. CM-III will also communicate with Data Network Technologies (DNT) software (STRAITBIZARRE) through a covert channel implemented on the USB, using this communication channel to pass commands and data between hardware and software implants. CM-III will be a GENIEcompliant implant based on CHIMNEYPOOL.
(TSI/SII/REL) CM-III conceals digital components (TRINITY), a USB 2.0 HS hub, switches, and HOWLERMONKEY (HM) RF Transceiver within a RJ45 Dual Stacked USB connector. CM-I has the ability to communicate to other CM devices over the RF link using an over-theair protocol called SPECULATION. CM-III can provide a short range inter-chassis link to other CM devices or an intra-chassis RF link to a long haul relay subsystem.
![img-101.jpeg](img-101.jpeg)

[^0]
[^0]:    TOP SECRET//COMINT//REL TO USA, FVEY
![img-102.jpeg](img-102.jpeg)

# FIREWALK ANT Product Data 

(TSI/SII/REL) FIREWALK is a bidirectional network implant, capable of passively collecting Gigabit Ethernet network traffic, and actively injecting Ethernet packets onto the same target network.
![img-103.jpeg](img-103.jpeg)
(TSI/SII/REL) FIREWALK is a bi-directional 10/100/1000bT (Gigabit) Ethernet network implant residing within a dual stacked RJ45 / USB connector. FIREWALK is capable of filtering and egressing network traffic over a custom RF link and injecting traffic as commanded; this allows a ethernet tunnel (VPN) to be created between target network and the ROC (or an intermediate redirector node such as DNT's DANDERSPRITZ tool.) FIREWALK allows active exploitation of a target network with a firewall or air gap protection. (TSI/SII/REL) FIREWALK uses the HOWLERMONKEY transceiver for back-end communications. It can communicate with an LP or other compatible HOWLERMONKEY based ANT products to increase RF range through multiple hops.
![img-104.jpeg](img-104.jpeg)

Status: Prototype Available - August 2008
Unit Cost: 50 Units $\$ 537 \mathrm{~K}$
![img-105.jpeg](img-105.jpeg)
![img-106.jpeg](img-106.jpeg)

# RAGEMASTER ANT Product Data 

(TS//SI//REL TO USA,FVEY) RF retro-reflector that provides an enhanced radar cross-section for VAGRANT collection. It's concealed in a standard computer video graphics array (VGA) cable between the video card and video monitor. It's typically installed in the ferrite on the video cable.

## (U) Capabilities

(TS//SI//REL TO USA,FVEY) RAGEMASTER provides a target for RF flooding and allows for easier collection of the VAGRANT video signal. The current RAGEMASTER unit taps the red video line on the VGA cable. It was found that, empirically, this provides the best video return and cleanest readout of the monitor contents.
![img-107.jpeg](img-107.jpeg)

## (U) Concept of Operation

(TS//SI//REL TO USA,FVEY) The RAGEMASTER taps the red video line between the video card within the desktop unit and the computer monitor, typically an LCD. When the RAGEMASTER is illuminated by a radar unit, the illuminating signal is modulated with the red video information. This information is re-radiated, where it is picked up at the radar, demodulated, and passed onto the processing unit, such as a LFS-2 and an external monitor, NIGHTWATCH, GOTHAM, or (in the future) VIEWPLATE. The processor recreates the horizontal and vertical sync of the targeted monitor, thus allowing TAO personnel to see what is displayed on the targeted monitor.

## Unit Cost: $\$ 30$

Status: Operational. Manufactured on an as-needed basis. Contact POC for availability information.
![img-108.jpeg](img-108.jpeg)
