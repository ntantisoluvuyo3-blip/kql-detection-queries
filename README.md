# KQL Detection Queries for SOC Analysts

A collection of production-ready Kusto Query Language (KQL) detection queries 
for Microsoft Sentinel and Azure Log Analytics.

## Overview

This repository contains detection queries covering common attack patterns 
and security scenarios that SOC analysts monitor daily in real-world environments.

## What's Included

### Credential Access Attacks
- **01-brute-force-detection.kql** - Password spray and brute force attacks
  - MITRE: T1110.003
  - Detects: Multiple failed logins from single IP targeting multiple users
  - Severity: High

### Coming Soon (14 more queries)
- Privilege escalation detection
- Lateral movement detection
- Data exfiltration detection
- Credential theft detection
- Malware indicators
- Persistence mechanisms
- And more!

## How to Use These Queries

### In Microsoft Sentinel:

1. Open your Sentinel workspace
2. Go to **Logs** section
3. Copy the entire query from any .kql file
4. Paste into the query editor
5. Click **Run** to test
6. Adjust timeframes and thresholds for your environment
7. Deploy as an **Analytics Rule** for automated alerts

### Customization:

Each query includes tuning parameters:
- **Thresholds** (5+ attempts, 3+ users, etc.) - adjust based on your risk tolerance
- **Timeframes** (ago(1h), ago(24h)) - modify for different detection windows
- **Severity levels** - change based on your environment

## MITRE ATT&CK Coverage

| Query | Technique | Tactic | Severity |
|-------|-----------|--------|----------|
| 01-brute-force-detection.kql | T1110.003 | Credential Access | High |

## Why These Queries Matter

✅ **Real-world applicable** - Based on actual SOC analyst workflows  
✅ **MITRE-mapped** - Each query aligns with attack techniques  
✅ **Production-ready** - Can be deployed directly to Sentinel  
✅ **Tunable** - Thresholds and timeframes adapt to your environment  
✅ **Well-documented** - Comments explain every step  

## Interview Value

These queries demonstrate:
- Log analysis and pattern recognition
- Threat detection methodology
- MITRE ATT&CK framework knowledge
- Practical Sentinel/KQL expertise
- Security operations thinking

## Query Structure

Each query file includes:
- **Header**: Query name, MITRE technique, severity, author, date
- **Description**: What the query detects and why it matters
- **KQL Logic**: The actual detection query with comments
- **Tuning Parameters**: How to customize thresholds for your environment

## Next Steps

This project will expand to include 15+ queries covering:
- All major attack tactics
- Real SOC analyst use cases
- Practical detection scenarios

## Created By

**Luvuyo Prince Ntantiso**  
July 2026

---

*Portfolio project demonstrating KQL and threat detection expertise*
