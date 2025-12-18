# SOC Incident Report – Failed Login Spike

## Summary
On 2025‑03‑25 at 14:25 UTC, the Splunk alert “Failed Login Attempts” triggered with >15 attempts from 192.0.2.25.

## Affected System
- Host: web‑server‑01
- Source IP: 192.0.2.25

## Analysis
- User accounts targeted: admin, user1
- Pattern indicates brute force behavior.

## Remediation Steps
1. Block IP at firewall.
2. Reset passwords for targeted accounts.
3. Enforce MFA for all admin & critical accounts.

## Prevention
- Enable IP reputation blocklists
- Tighten login thresholds on Splunk
