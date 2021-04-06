---
title: Cyber Kill Chain - Explained
tags: [Information Security,Cyber Attack,Knowlegde]
published: true
description: A series of steps that trace the stages of a cyberattack from the early reconnaissance stages to the exfiltration of data.
toc: true
image: https://i.pinimg.com/originals/7a/b0/b8/7ab0b884b7050bbae9cc976409cd5567.png
thumbnail: https://i.pinimg.com/originals/7a/b0/b8/7ab0b884b7050bbae9cc976409cd5567.png
---

The cyber kill chain is a series of steps that trace the stages of a cyberattack from the early reconnaissance stages to the exfiltration of data. Understanding this model can help IT security teams put strategies and technologies in place to “kill” or contain a cyber-attack or APT(Advanced Persistent Threat) at various stages, and better protect the IT ecosystem.

'Kill chain' is a term originally used by the military to define the steps an enemy uses to attack a target. In 2011, Lockheed Martin adapted this concept to Information Security and named it Cyber Kill Chain.

## 7 Steps of Cyber Kill Chain
Lockheed Martin’s cyber kill chain breaks down a cyberattack into 7 distinct steps: 
![Cyber Kill Chain](../assets/images/cyber_kill_chain.png)

### 1. Reconnaissance
The observation stage: attackers typically assess the situation from the outside-in, in order to identify both targets and tactics for the attack, it’s the preliminary step of an attack. During reconnaissance, an attacker is seeking information that might reveal vulnerabilities and weak points in the system. Firewalls, intrusion prevention systems, perimeter security, even social media accounts – get ID’d and investigated. Reconnaissance tools scan corporate networks to search for points of entry and vulnerabilities to be exploited.

On the defensive side, the Security team of an organization can stop the hacker or an attack to occur by hiding sensitive information and monitoring for simple thresholds, such as a number of ports connected to single-origin over a period of time. IDS and firewalls can be configured to detect network and port scans.

### 2. Weaponization
This step happens at the attacker's side. After Reconnaissance attacker may have information about what services are running on the target, which systems they work on, what ports are open, what is physical security or they may have physical access to the building.
Based on all this information, the attacker creates a malicious payload to exploit the vulnerability found in the Reconnaissance step.

There are few security controls, including security awareness, that may impact or neutralize this stage. The security team has to be updated with recent exploits, updating systems and services regularly.

### 3. Delivery
This is the phase where the malicious payload is sent to the target. This can be done through Social Engineering like sending out phishing emails, dropping infected USB drives outside the building, cafe, etc. There are other ways of doing this also like if there's an FTP server configured by the target, through attacker can send the payload after getting credentials or anonymously also if the server is not configured properly. Also, an attacker can send it through some upload form that may be present on the website of the target.

The attack can be "killed" at this stage by using proper input validation and sanitization of data whenever taking input from the user and properly training employees and making them aware of social engineering.   

### 4. Exploitation
The objective at this stage is to exploit the vulnerability by executing the payload attacker delivered to the target. 

Trained people ensure the systems they are running are updated and current. They ensure they have anti-virus running and enabled. They ensure that any sensitive data they are working with is on secured systems, making them far more secure against exploitation. 

### 5. Installation
The attacker installs malware on the victim. Not all attacks require malware, such as a CEO fraud attack or harvesting login credentials. Attackers at this stage can now get into the system and install additional tools, modify security certificates, and create new script files for nefarious purposes.

A trained and secure workforce can help ensure they are using secure devices that are updated, current, and have anti-virus enabled, which would stop many malware installation attempts. A key step in detecting an infected system is to look for abnormal behavior.

### 6. Command and Control (C2)
This implies that once a system is compromised and/or infected, the system has to call home to a Command and Control (C2) system for the cyber attacker to gain control. Typically, compromised hosts must beacon outbound to an Internet controller server to establish a C2 channel. Once the C2 channel establishes, intruders effectively have “hands on the keyboard” access inside the target environment. The trick for attackers is to have established control over many work stations in an effort to “exfiltrate” data without setting off any anomalies or other monitoring applications based upon content, quantity, frequency, etc.

This stage is the defender’s “last best chance” to block the operation: by blocking the Command and Control channel. Hence, the reason it is essential to have the proper tools in place that can identify, track, observe, stop, and destroy these campaigns within defending capabilities.

### 7. Actions on Objective
The longer an adversary has this level of access, the greater the impact.  Defenders must detect this stage as quickly as possible and deploy tools that will enable them to collect forensic evidence. One example would include network packet captures, for damage assessment.


### Resources
- [Lockheed Martin's White Paper](https://www.lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf)
- [SANS Security Awareness](https://www.sans.org/security-awareness-training/blog/applying-security-awareness-cyber-kill-chain)
- [Varonis- Cyber Kill chain](https://www.varonis.com/blog/cyber-kill-chain/)