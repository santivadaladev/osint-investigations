# PEC Phishing Campaign Analysis & Incident Response

A comprehensive Threat Intelligence and Incident Response analysis of a massive phishing campaign targeting Italian Certified Email (PEC) users. This project demonstrates log analysis, infrastructure mapping, and official abuse reporting workflows.

## 🎯 Case Overview

An attacker launched a coordinated phishing campaign disguised as a security alert from a major digital banking service. By leveraging a compromised corporate PEC account, the threat actor bypassed standard email security controls (SPF/DKIM Hard Fails) to target hundreds of businesses.

- **Threat Type**: Social Engineering / Financial Phishing
- **Attack Vector**: Compromised Certified Email (PEC) Infrastructure
- **Delivery Mechanism**: Massive direct distribution via exposed `To:` fields
- **Status**: **Mitigated** (Infrastructure successfully dismantled)

---

## 🔍 Technical Analysis & Investigation

### 1. Header Analysis (Email Vector)
Initial inspection of the raw email headers revealed a critical mismatch between the spoofed brand and the authenticated sender:

```text
Subject: [TARGET_BRAND]: Verify your account
From: [COMPROMISED_ORGANIZATION] <REDACTED@legalmail.it>
Received: from internal-webmail-node (IP: 10.x.x.x) by sendm.cert.legalmail.it
Authentication-ID: M63XXXXX@userid.local
```

**Key Insight:** Security boundaries were bypassed because the attacker didn't spoof the domain names. Instead, they compromised legitimate credentials on an official PEC account, utilizing the trusted provider's SMTP servers to guarantee delivery.

### 2. DNS & Domain OSINT
Investigating the phishing landing page through Kali Linux CLI tools (`dig`, `whois`) revealed the lifecycle and current state of the malicious domain:

```bash
$ dig MX [REDACTED_PHISHING_DOMAIN].in @8.8.8.8
;; ->>HEADER<<- opcode: QUERY, status: NXDOMAIN

$ whois [REDACTED_PHISHING_DOMAIN].in | grep "Domain Status"
Domain Status: clientHold
Domain Status: clientTransferProhibited
```

**Key Insight:** The domain status `clientHold` confirms that the upstream registrar suspended the domain due to malicious activity shortly after detection, removing it from global DNS zones and neutralizing the threat.

### 3. Infrastructure Mapping
Tracing the Authoritative Name Servers linked back to a high-volume, low-cost hosting registrar:

- **Registrar**: Tucows Domains Inc.
- **Reseller/Hosting Provider**: Qwikserver (India)
- **Infrastructure Age**: Active since 2021 (indicating shared or bulletproof infrastructure rather than custom-built for this single campaign).

---

## 🛡️ Incident Response Action Taken

To mitigate ongoing risk and protect potential victims, the following structured response was executed:

1. **Threat Intelligence Extraction**: Extracted and sanitized a database of 250+ targeted corporate email addresses.
2. **Provider Notification (Abuse)**: Drafted and dispatched an official incident report to the Certified Email provider containing the compromised account IDs (`M63XXXXX`) to initiate an immediate credential reset.
3. **Brand Alert**: Forwarded the network Indicators of Compromise (IoCs) to the impersonated financial institution for transactional monitoring.

---

## 📊 Indicators of Compromise (IoCs)

```text
# Campaign Indicators - Sanitized Format
domain|[REDACTED_MALICIOUS_DOMAIN].in
email-src|[REDACTED_COMPROMISED_ACCOUNT]@legalmail.it
email-subject|[BRAND_NAME]: Verifica il tuo account
nameserver|ns1.serverbyt.xx
nameserver|ns2.serverbyt.xx
source-ip|10.227.xx.xx (Internal Webmail Node)
```

---

## 🛠️ Tools Used
- **OS**: Kali Linux
- **Network Diagnostics**: `dig`, `nslookup`
- **Reconnaissance**: `whois`
- **Data Parsing**: `grep`, `regex`, Bash text-processing utilities

---
*Disclaimer: All sensitive data, personally identifiable information (PII), and live malicious URLs have been redacted or anonymized in compliance with responsible disclosure guidelines.*
