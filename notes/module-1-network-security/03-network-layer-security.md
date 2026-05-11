# Network Layer Security

## Overview

The network layer is responsible for routing, addressing, and delivering packets between different networks.

Because this layer controls traffic flow and communication paths, it is common target for attacks that attempt to redirect, manipulate, or disrupt network traffic.


# Common Network Layer Attacks

## BGGP Hijacking

This occurs when an attacker manipulates the Border Gateway Protocol (BGP) to redirect internet traffic through malicious or unauthorized routes.

Possible consequence:

- Traffic intercerption.
- Traffic redirection.
- Service disruption.
- Data monitoring.


## Ping of Death

This sends oversized ICMP packets that exceed the target system´s buffer capacity, potentialy causing crashes or instability.

Impact:

- System crashes.
- Services disruption.
- Denial of Service (DoS).

Modern systems are generally protected against this attack, but it remains an important historical example.


## IP Spoofing

Consists of forging the source or destination IP address within packet headers to impersonate another systems.

Possible objetives:

- Bypass filtering mechanisms.
- Hide attacker identidy.
- Launch reflection or amplification attacks.


# Protection Mechanisms

## 1. IPsec:

Encrupts and authenticates network packets while providing secure communication between systems.

Common uses:

- VPN connections.
- Secure site-to-site communication.
- Data integrity protection.

Benefits:

- Confidentiality.
- Integrity.
- Authentication.


## 2. Network-Based IDS/IPS

Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS) analyze network traffic to detect and block suspicious activity.

They inspect fields such as:
- Source IP addresses
- Destination IP addresses
- Protocol behavior
- Traffic patterns

---

## 3. DDoS Protection

Organizations use different techniques to mitigate Distributed Denial of Service (DDoS) attacks.

Examples:
- Load balancers
- IP block lists
- Traffic filtering
- Rate limiting

---

# Importance

Network layer security is essential because attackers often target routing and packet delivery mechanisms to intercept traffic, hide malicious activity, or disrupt services.

---

# Personal Insight

Understanding network layer attacks helps build stronger defenses against traffic manipulation, spoofing, and denial-of-service attacks commonly seen in real-world environments.