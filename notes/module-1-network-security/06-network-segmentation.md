# Network Segmentation

## Overview

Network segmentation consists of dividing a network into smaller and isolated segments in order to improve security, monitoring, and access control.

Proper segmentation reduces the attack surface and limits lateral movement within an organization.

---

# Example Enterprise Architecture

A typical enterprise network may contain multiple isolated environments.

## Intranet

Internal corporate infrastructure:
- Workstations
- Internal servers
- Secondary devices
- IoT devices
- Internal firewall
- IDS/IPS systems

---

## DMZ (Demilitarized Zone)

Services exposed to the internet:
- Public websites
- VPN servers
- Customer applications

Security components:
- WAF
- External firewall

---

## External Entities

The network may also interact with:
- Internet users
- Remote employees
- Cloud services
- External attackers

---

# Types of Network Segmentation

## Physical Segmentation

Uses dedicated physical devices to separate network segments.

Examples:
- Switches
- Routers
- Firewalls

### Advantages
- Complete isolation
- High security

### Disadvantages
- High cost
- Low scalability

---

## Logical Segmentation

Logical segmentation divides networks digitally using subnets and VLANs.

### Advantages
- Lower cost
- High scalability
- Easier monitoring

### Disadvantages
- Lower isolation
- Requires secure configuration

---

## Microsegmentation

Microsegmentation applies granular security controls at the device, application, or user level.

### Advantages
- Ideal for cloud and virtualized environments
- High scalability

### Disadvantages
- Complex implementation
- Requires advanced infrastructure

---

# Best Practices

## Guest Networks

Guest networks provide internet access for external users while remaining isolated from the corporate infrastructure.

Characteristics:
- Isolated from internal systems
- Internet access only
- Low-level monitoring within legal regulations

---

## IoT Networks

IoT devices are often isolated from the main corporate network.

Examples:
- CCTV cameras
- Smart TVs
- OT devices

Security measures:
- Restricted internet access
- Block inbound connections
- Monitor for external attacks and Data Loss Prevention (DLP)

---

## Legacy Systems

Legacy systems often run outdated and vulnerable operating systems while controlling critical machinery or processes.

Security recommendations:
- Complete isolation
- Strict communication controls
- Defined data extraction procedures
- Monitoring through updated intermediary devices

---

## Demilitarized Zone (DMZ)

The DMZ contains services exposed to the internet.

Examples:
- Websites
- Forums
- Customer support systems
- VPN servers

Characteristics:
- Internet access filtered through firewalls
- Controlled access to internal networks
- Strong authentication mechanisms
- High monitoring using WAF and other security tools

---

## Corporate Network

The corporate network contains:
- Workstations
- Internal servers
- Internal business services

Best practices:
- Firewall-filtered internet access
- Segmentation into subnets
- Least privilege policies
- High-level monitoring

---

## Air-Gapped Systems

Air-gapped systems require maximum security and are isolated from other networks.

Characteristics:
- No internet connectivity
- Physical or logical isolation
- Reduced data exfiltration risk
- Contained infections in case of compromise

Despite isolation, these systems still require strong monitoring and security controls.

---

# Importance

Network segmentation is critical because it limits lateral movement, improves visibility, and protects sensitive systems from unauthorized access.

---

# Personal Insight

Proper segmentation is one of the most effective defensive strategies in cybersecurity because it prevents attackers from easily moving across the infrastructure after compromising a system.