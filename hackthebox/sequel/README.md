Hack The Box – Sequel Write-up

Overview

This write-up documents the analysis of the Hack The Box "Sequel" machine.
The objective was to enumerate exposed services, identify database-related
misconfigurations, and demonstrate how weak or exposed credentials can lead
to unauthorized access in an authorized lab environment.

Scope
Target: Hack The Box – Sequel

Operating System: Linux

Difficulty: Starting Point / Very Easy

Goal: Gain system-level access and retrieve the final flag

Enumeration
Initial enumeration revealed a database service exposed to the network.
Such services are not typically intended to be directly accessible without
strong authentication and access controls.

Due to the nature of the exposed service, further enumeration focused on
authentication behavior and potential misconfigurations related to database access.

Vulnerability Analysis
The primary issue was an insecure database configuration.
In this scenario, the database service allowed authentication using weak,
default, or easily guessable credentials.

This type of vulnerability commonly occurs when:

Default credentials are not changed

Database services are unnecessarily exposed

Access controls are misconfigured or absent

Exploitation (High-level)
Within the authorized HTB lab environment, database access was achieved using
identified credentials. This access allowed further interaction with the system
and ultimately led to system-level access and retrieval of the final flag.

Note: Specific commands and exploitation steps are intentionally omitted to
prevent misuse outside legal lab environments.

Impact
An attacker gaining unauthorized access to a database service may:
Access or manipulate sensitive data
Extract credentials stored within the database
Escalate privileges and compromise the underlying system
In enterprise environments, such exposure can lead to data breaches,
service disruption, and full infrastructure compromise.

Mitigation
Restrict database services to internal or trusted networks only
Enforce strong, unique credentials and disable default accounts
Apply least privilege to database users
Regularly audit exposed services and configurations
Monitor authentication attempts and access patterns

Detection Ideas (Blue Team)
Alert on database authentication attempts from unexpected sources
Monitor repeated failed or anomalous login attempts
Correlate database access events with subsequent system activity
