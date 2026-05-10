# Access Layer Security

## Overview

The access layer is responsible for connecting devices to the local network.

This layer includes switches, wireless access points, and endpoint devices. Because it operates close to users and devices, it is commonly targeted by local network attacks.


# Common Access Layer Attacks

## MAC Spoffing

MAC Spoffing consists of manually changing the attacker`s MAC address to impersonate another device on the network.

Posibles objetives:

- Bypass MAC filtering.
- Impersonate trusted devices.
- Gain unauthorized network access.


## ARP Poisoning

ARP Poisining (or ARP Spoofing) involves sending forged ARP packets to convince devices that the attacker´s machine in the legitimate router or another trusted device.

Possible consequences:

- Man-in-the-Middle (MITM) attacks.
- Traffic interception.
- Credential theft.
- Network disruption.


## Switch Port Hijacking

This attack abuses MAC spoofing and ARP manipulation to take control of a switch port and receive traffic intended for another device.

Posible impact:

- Traffic sniffingg.
- Session interception.
- Unauthorized monitoring.


# Protection Mechanisms

## 1. Access Control

### 802.1X / NAC

802.1X and Network Access Control (NAC) authenticate devices before allowing them to connect to the network.

Benefits:

- Prevent unauthorized devices.
- Improved visibility and control.
- Enforce security policies.


## WPA3

Provides stronger wireless authentication and encryption for WIFI networks.

Benefits:

- Improved password protection.
- Better encryption.
- Protecction against brute-force attacks.


## 2. Switch Port Protection

Switch security mechanisms can limit the number of MAC addresses associated with a single switch port.

Benefits:

- Prevent MAC flooding attacks.
- Restrict unauthorized devices.
- Improve network control.


### 3. MAC Filtering

Restricts network access to approved MAC addresses.

Limitation:

MAC addresses can still be spoofed, so this should not be the only security mechanism.


# Importance

Access layer security is essential because attackers who gain local network access may intercept traffic, impersonate devices, or move laterally through the infraestructure.


# Personal Insight

Many internal network attacks begin at the access layer, making proper switch security, authentication, and monitoring critical components of a secure infrastructure.
