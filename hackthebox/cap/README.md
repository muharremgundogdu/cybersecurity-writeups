# Hack The Box - Cap Write-up

## Overview
This write-up documents the analysis and exploitation of the Hack The Box "Cap" machine.
The objective was to analyze exposed services and identify sensitive information leakage
from captured network traffic.

## Scope
- Target: Hack The Box - Cap
- OS: Linux
- Difficulty: Very Easy
- Goal: Gain user and root access

## Enumeration
An initial port scan was performed to identify exposed services on the target system.
The scan revealed a web service running on port 80, which became the primary focus
for further enumeration.

Upon visiting the web application, multiple network capture (PCAP) files were discovered.
These files appeared to be accessible without authentication, indicating a potential
information disclosure issue.

## Vulnerability Analysis
The web application exposed multiple PCAP files that contained captured network traffic.
One of these captures included sensitive information transmitted in cleartext.

The root cause of the vulnerability was the lack of proper access control and encryption,
allowing attackers to analyze network traffic and extract credentials.

## Exploitation

## Impact

## Mitigation
