# Endpoint Security

## What is an Endpoint?

### Definition

1. Any device connected to a network that can become the victim of a cyberattack.

2. Endpoints must be identifiable through attributes such as:
- IP address
- MAC address
- UUID

3. Endpoints provide some type of:
- User interface
- Service
- Network functionality

---

# Threat Protection Lifecycle

## Threat Detection

- Detection mechanisms are based on:
  - Suspicious behaviors
  - Indicators of Compromise (IOCs)

- Detection can be:
  - Static
  - Dynamic

---

## Threat Reporting

- Threats are reported to:
  - Security systems
  - SOC teams
  - Incident response teams

- Enables investigation and response activities.

---

## Threat Response

- Threat containment and blocking.
- Endpoint isolation if required.

---

## Remediation and Protection

- Threat analysis and eradication.
- DFIR (Digital Forensics and Incident Response) processes.

---

# Antivirus (AV)

1. Detection based on heuristic models:
- Known hashes
- Malicious domains
- IP addresses
- URLs

2. Limited response capabilities:
- Process termination
- Quarantine

3. Lower resistance against sophisticated attacks.

4. Designed to operate autonomously.

---

# Endpoint Detection and Response (EDR)

1. Uses hybrid detection models:

### Static Detection
- Traditional AV techniques
- Fuzzy hashing

### Dynamic Detection
- Behavioral analysis
- Event correlation
- AI-enhanced detections

---

2. Low-level process monitoring:
- Higher resource consumption

3. Advanced response capabilities:
- Rollback features
- Endpoint isolation

4. Higher resistance against advanced threats.

5. Requires SOC analysts for investigation and response.

---

# Exposure Reduction

# Application Control

## Allow / Deny Lists

Applications can be allowed or blocked based on:
- Hashes (MD5, SHA1, SHA256)
- Digital certificates
- Specific paths or directories

---

## Script Execution Control

Blocking execution of:
- Bash
- PowerShell
- Python
- Other scripting languages

Based on:
- Users
- Groups
- Policies

---

## Vulnerable Drivers

- Blocking installation or execution of vulnerable drivers.

---

# Device Control

1. Blocking physical devices:
- USB drives
- External disks
- Peripherals

2. Prevents:
- Device mounting
- Driver installation

3. Supported by some EDR solutions.

---

# Network Control

# Host-Based Firewall

- Filters inbound and outbound traffic.
- Can filter traffic by application.

---

# DNS Filtering

- DNS requests are redirected through controlled DNS servers.
- Only approved domains are resolved.

---

# Corporate VPN

- Forces traffic through secure VPN tunnels.
- Enables monitoring and filtering of network traffic.

---

# Additional Recommended Measures

## Updates

- Keeping operating systems and applications updated helps prevent exploitation of vulnerabilities.

---

## Authentication

- Principle of least privilege
- Strong passwords
- Multi-Factor Authentication (MFA)

---

## Configuration

- Avoid exposing unnecessary services:
  - RDP
  - SSH
  - FTP

- Review default configurations.

---

# Increasing Visibility

# Logging and Auditing

- Increase logging activities.
- Extend log retention periods.

Logs may come from:
- Operating systems
- Applications
- Services

---

# Security Information and Event Management (SIEM)

- Centralizes logs from multiple systems.
- Enables:
  - Correlation
  - Monitoring
  - Threat detection

---

# Data Loss Prevention (DLP)

- Monitors sensitive information.
- Prevents:
  - Data leaks
  - Unauthorized transfers
  - Exfiltration

---

# System Integrity Protection

# Disk Encryption

- Full disk encryption protects against data theft in case of physical compromise.

---

# Secure Boot

- Verifies that:
  - Bootloaders
  - Kernels
  - Drivers

are digitally signed and trusted.

---

# BIOS / UEFI Protection

- BIOS/UEFI passwords
- Disable boot from external devices
- Maintain immutable boot order

---

# Security by Operating System

# Windows

- Advanced security technologies available
- High probability of being targeted
- Users commonly have administrative privileges
- Complex configuration

---

# Linux

- Strong security ecosystem
- Large amount of open-source security tools
- Common target in servers and containers
- Root access should be restricted to IT personnel

---

# iOS

- Strong integrated security
- Strict application isolation
- Lower exposure except through social engineering
- Limited customization

---

# Android

- Security varies between manufacturers
- Sandboxing between applications
- Higher exposure risk
- Limited management capabilities compared to desktop operating systems

