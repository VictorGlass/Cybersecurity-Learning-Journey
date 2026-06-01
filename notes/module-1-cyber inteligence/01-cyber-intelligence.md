# Cyber Intelligence (CTI)

## Introduction — What is Cyber Intelligence?

Cyber Intelligence (Cyber Threat Intelligence - CTI) is intelligence focused on understanding threats present in the digital environment.

The purpose of CTI is to transform raw data into actionable intelligence that supports decision-making and security operations.

---

## Data → Information → Intelligence

### Data

Raw and unstructured information collected from multiple sources.

Characteristics:
- Large volume
- Multiple sources
- Not structured

Examples:
- Logs
- IP lists
- Security events

---

### Information

Processed and structured data.

Characteristics:
- Centralized
- Normalized
- Organized

Examples:
- Databases
- Aggregated security events

---

### Intelligence

Information that has been processed and analyzed to generate actionable knowledge.

Examples:
- IP addresses associated with an APT group
- Threat campaign analysis

---

# Intelligence Sources

Typical resources used by CTI processes:

- Threat intelligence exchange platforms
- Open Source Intelligence (OSINT)
- Geopolitical intelligence
- Human Intelligence (HUMINT)
- Malware analysis
- Indicators of Compromise (IOCs)
- Social networks
- Internal information (SIEM, EDR, previous incidents)
- Deep Web / Dark Web
- Messaging platforms (Telegram, WhatsApp)

---

# Intelligence Lifecycle

Cyber Threat Intelligence follows a structured lifecycle.

## 1. Planning

Define:

- Objectives
- Requirements
- Scope of the intelligence exercise

---

## 2. Collection

Select sources and gather relevant data.

---

## 3. Processing

Transform collected data into structured and normalized information.

---

## 4. Analysis

Apply formal analysis methodologies to generate actionable intelligence.

---

## 5. Dissemination

Deliver intelligence products to the appropriate stakeholders.

---

# Types of Intelligence

## Strategic Intelligence

Provides a high-level view of:

- Threat landscape
- Risks
- Emerging trends

Closely linked with risk management processes.

Audience:
- Executives
- Leadership teams

---

## Tactical Intelligence

Provides detailed information about:

- Threat Actor TTPs
- Attack methods
- Defensive opportunities

Audience:
- Security specialists
- SOC Managers
- Technical teams

---

## Operational Intelligence

Focuses on identifying attack patterns in real time.

Objectives:

- Correlate malicious activities
- Identify attackers
- Support incident response

Audience:
- DFIR teams

---

## Technical Intelligence

Provides low-level indicators such as:

- IP addresses
- URLs
- Domains
- Malware hashes

Objectives:

- Enable real-time detection
- Automate monitoring systems

Note:
This type of intelligence has a shorter operational lifespan.

---

# Cyber Kill Chain

Cyber Kill Chain describes the phases of a cyberattack.

(Model developed by Lockheed Martin)

## 1. Reconnaissance

Identify and investigate the target.

---

## 2. Weaponization

Select attack vectors and prepare malicious payloads.

---

## 3. Delivery

Deliver malware through selected channels.

---

## 4. Exploitation

Execute the initial compromise.

---

## 5. Installation

Establish persistence and maintain control.

---

## 6. Command and Control (C2)

Establish communication with attacker-controlled infrastructure.

---

## 7. Actions on Objectives

Achieve the final objective.

---

# Tactics, Techniques and Procedures (TTPs)

## Tactics

High-level description of attacker objectives.

Example:
- Establish Persistence

---

## Techniques

Methods used to achieve tactical objectives.

Example:
- Persistence through Windows Registry

---

## Procedures

Specific implementation details.

Example:
- Persistence through RunOnce Registry Key

---

## MITRE ATT&CK Framework

MITRE ATT&CK provides a knowledge base of adversary behavior.

It maps:

- Tactics
- Techniques
- Procedures

Used extensively for:

- Detection
- Threat Hunting
- Intelligence Reporting

---

# Advanced Persistent Threats (APTs)

APT groups usually operate with long-term objectives.

## Motivations

### State-Sponsored Groups
- Political
- Espionage
- Destructive objectives

### Hacktivists
- Political motivation

### Cyber Criminals
- Financial gain
- Disruption

---

## Common Naming Sources

Different vendors assign different group names.

Examples:

- CrowdStrike
- Unit 42
- MITRE
- Mandiant

---

# Intelligence Dissemination

## STIX and TAXII Standards

---

### STIX — Structured Threat Information eXpression

Structured language designed for cyber threat intelligence exchange.

Capabilities:

- Describe complex threat information
- Represent attacker capabilities
- Document motivations

---

### TAXII — Trusted Automated Exchange of Intelligence Information

Protocol designed to exchange CTI data.

Features:

- Built as an API model
- Designed for STIX transport
- Supports multiple distribution models

Models:

#### Collection
Request/Response model

#### Channel
Subscription-based intelligence feeds

---

# CTI Platforms

## OpenCTI

Open-source platform for:

- Intelligence ingestion
- Analysis
- Dissemination

Capabilities:

- External source enrichment
- Custom TAXII feeds
- STIX export
- Reporting

---

## MISP (Malware Information Sharing Platform)

Open-source platform for collaborative intelligence sharing.

Features:

- Import/export intelligence
- STIX support
- Widely adopted by organizations

Examples:
- RNS
- FIRST
- NATO

---

# CTI Use Cases

## Threat Hunting and Continuous Monitoring

### Threat Hunting

Provides hypotheses to guide proactive investigations.

### Continuous Monitoring

Supports:

- Use case creation
- Alert enrichment
- Context expansion

---

## DFIR and Malware Analysis

### DFIR

Supports:

- Incident investigation
- Attribution
- Response orientation

### Malware Analysis

Enables:

- Malware family identification
- Detection rule creation
- MITRE ATT&CK mapping

---

## Attack Surface Management (ASM)

Analyzes infrastructure to identify possible entry points.

Uses:

- Known TTPs
- External exposure analysis

---

## Purple Team

Coordinates collaboration between:

- Red Team (Attack)
- Blue Team (Defense)

Objective:

Improve detection and defensive capabilities through joint operations.