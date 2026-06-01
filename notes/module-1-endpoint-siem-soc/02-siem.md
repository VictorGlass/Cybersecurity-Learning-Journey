# SIEM

## What is SIEM

### Security Information and Event Management

1. Collects logs from multiple services across the organization:
   - Firewall
   - Applications
   - Endpoint Events
   - Windows Events
   - Active Directory
   - EDR

2. Processes and analyzes this information in real time to detect and report suspicious activities.

3. Correlates events and alerts to group related activities together.

4. The cost of these tools is usually defined by:
   - Data ingestion volume
   - Log retention period


---

## Data Ingestion

### What can we ingest?

- Firewall
- Active Directory
- Applications
- IDS / IPS
- CTI (Cyber Threat Intelligence)

- Endpoint Events
- Cloud Services
- EDR
- Physical Sensors
- WAF


### Data Normalization


Common Event Format (CEF)
    ↓
Common Log Format
    ↓
Extended Log Format (ELF)
    ↓
CSV
    ↓
Custom Formats
    ↓
SYSLOG
    ↓
RAW
    ↓
Windows Event Logs (EVTX)
    ↓
XML
    ↓
JSON


## Log Filtering Methods

### What do we record?

- During log generation, organizations must decide which events should be logged and which should not.
- Decisions depend on:
Software development
Application and service configuration
Security requirements
Regulatory compliance
- Logging levels, retention policies, and log rotation must also be considered.


### What do we send?

From all generated events, organizations select which logs should be forwarded to the SIEM.

### Examples:

- Windows Security Events
- Critical application events
- DNS resolution logs

Only relevant information should be transmitted to support:

- Security operations
- Auditing
- Monitoring


### What do we store?

From received events, only selected logs become part of long-term retention.

#### Examples:

- Specific Event IDs
- Traffic from critical servers

#### Stored logs should support:

- Continuous monitoring
- DFIR investigations
- Regulatory auditing


## Monitoring

### Use Cases

INFO
- Disk usage > 80%

Example:

- Reduced storage capacity for the database of a security tool.

LOW
- Shared SharePoint folder deleted

Example:

- Deletion of a folder shared with multiple users.

MEDIUM
- Creation of a privileged user

Example:

- Creation of a user with administrative permissions.

HIGH
- Successful login from an unusual country

Example:

- Login from a rare geographic location and suspicious IP address.

CRITICAL
- Critical server outage

Example:

- Loss of ingestion and heartbeat from the organization's main server for more than one hour.

LOW
- Multiple failed login attempts

Example:

- Possible password brute force attempt against a user protected with MFA.


### Use Cases

Naming Convention

How do we identify use cases?

- Names
- Codes (Example: UMMA-0001)
- UUIDs


Typology

What types of use cases exist?

Service Health Monitoring

Examples:

- Supported EDR agent versions
- Continuous ingestion monitoring
- Threat Detection

Examples:

- Malware detection
- Successful login monitoring


## Proactive Hunting

Examples:

- Zero-days
- Specific CVEs
- Incident-related IOCs

