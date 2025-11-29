# ev-charging-station-security

This repository delves into the cybersecurity challenges surrounding electric vehicle (EV) charging infrastructure, analyzing the security vulnerabilities in charging stations, communication protocols, and potential attack vectors that could compromise the charging process.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Background](#background)
3. [Security Analysis](#security-analysis)
4. [Attack Demonstration Videos](#demo--video-walkthrough)
5. [Proposed Mitigations](#proposed-mitigations)
6. [Future Work](#future-work)
7. [Conclusion](#conclusion)

## Project Overview

This project explores the security risks within EV charging stations and their communication protocols, focusing on physical-layer vulnerabilities and how attackers can exploit weak authentication systems to manipulate charging behaviors. Our work highlights key flaws in widely-used charging protocols and presents the results of real-world attack demonstrations.

## Background

Electric vehicles (EVs) rely on secure charging stations for energy transfer. However, many existing charging systems, such as those based on the GB/T, IEC, and SAE J1772 standards, have weak authentication mechanisms. These weaknesses create significant security risks, allowing attackers to spoof authentication signals, lock charging ports, or even compromise vehicle systems through the charging interface.

## Security Analysis

We identify and analyze various vulnerabilities in the authentication circuits of EV charging systems. These vulnerabilities stem from the use of static impedance and simple PWM signals for authentication, which can be easily spoofed by an attacker with physical access to the charging gun.

The primary security concerns include:

* Impersonation of charging states through spoofed resistance or PWM signals.
* Injection of malicious commands into the charging protocol, allowing remote control of the charging process or vehicle systems.

## Demo / Video Walkthrough

We also provide a collection of demonstration videos showcasing attack scenarios, experimental setups, and real‑world tests. You can find them in the following playlist:

**[EV Charging Station Security Demo Videos](https://youtube.com/playlist?list=PLcPx5A14HPko503cdxymPkMIsqWhoEMrI&si=rrWrpdEu_EWWiw2s)**

These videos include:

* Physical‑layer spoofing attacks against EV charging connectors.
* Device prototype deployment and operation (our "proof‑of‑concept" hardware).
* Attack results on different charger/vehicle models.
* Safety/disclosure considerations around EV charging security.

## Proposed Mitigations

To mitigate the risks associated with weak authentication, we propose several solutions:

* **Memory Electric Elements**: Using memory-based components to introduce dynamic resistance behavior, making it harder for attackers to replicate valid states.
* **Dynamic Power Authentication**: Implementing dynamic impedance values that change in real-time during the charging session, preventing static spoofing attacks.

## Future Work

Future efforts will include:

* Expanding the PORTulator attack suite to test additional charging systems and standards.
* Conducting real-world testing under varied environmental conditions, including different charging loads and interference from other wireless devices.
* Investigating the impact of BMS (Battery Management System) protections on spoofing attacks and exploring ways to bypass these safety measures.

## Conclusion

Our research reveals significant vulnerabilities in the authentication mechanisms of widely-adopted EV charging protocols. By exploiting weaknesses in physical-layer communication, attackers can manipulate charging processes, lock vehicles, or even cause damage to critical systems. We have outlined potential countermeasures and future research directions to strengthen the security of EV charging infrastructure.

