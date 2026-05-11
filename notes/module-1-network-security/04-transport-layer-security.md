# Transport Layer Security

## Overview

The transport layer is responsable for end-to-end communication devices across a network.


Its main objetives include:

- Reliable data transmission.
- Connection management.
- Error handling.
- Data flow control.


The most common transport layer protocols are TCP and UDP.

# Common Transport Layer Attacks


## Port Scanning

Port scanning consists of itering through ports on a target device to identify open services and gather information about the system.


Attackers commonly use port scanning to:

- Discover exposed services.
- Identify vulnerabilities.
- Map network infraestructure.


Common tools:

- Nmap.
- Masscan.


## SYN Flood

A SYN Flood attack sends a large number of TCP SYN requests to exhaust the server´s connection buffer and prevent legitimate connections.

Impact:

- Service disruption.
- Denial of Service (DoS).
- Resource exhaustion.


## LAND attack

A LAND attack sends TCP SYN packets where the source and destination IP address and port are identical.

This may cause systems to enter loops or consume excessive resources.

Modern operating systems are generally protected against this attack.


# Protection Mechanisms

## 1. Firewalls:

Firewalls filter network traffic based on ports, protocols, IP address, and security rules.

Functions:

- Block unathorized ports.
- Restrict suspicious traffic.
- Control inbound and outbound connections.


## 2. Transport Layer Security (TLS):

TLS provides secure communication through:

- Authentication.
- Encryption.
- Integrity protection.

TLS commonly uses SSL/TLS certificates to verify the authenticity of systems and secure communcations.

Common uses:

- HTTPS.
- Secure email.
- VPN communications.

## 3. Secure Protocol Implementation:

Many transport-layer attacks can be prevented through proper protocol implementation and secure configurations.

Examples:

- Keeping systems updated.
- Disable insecure protocols.
- Using secure cipher suites.
- Applying rate limiting protections.


# Importance

Transport layer security is essential because attackers frequently target exposed services, insecure protocols, and weak network configurations.

# Personal Insight

Understanding transport layer attacks and protections is fundamental for identifying exposed services, analyzing traffic behavior, and securing network communications in real-world environments.
