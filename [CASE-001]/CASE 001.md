# CASE-001 · Operation Ghost Seller
**Type:** Network Fraud Analysis | **Target Sector:** Retail/Sportswear

## 1. Executive Summary
The investigation was triggered by the detection of a network of clone websites utilizing digital assets from a well-known Italian brand. The analysis successfully mapped an entire fraudulent infrastructure consisting of **6 interconnected domains**, with servers located in offshore jurisdictions and payment flows redirected toward Eastern Europe.

## 2. Infrastructure Mapping
### 🌐 Digital Asset Investigation

| Parameter | Result (Obfuscated) | Technical Notes |
| :--- | :--- | :--- |
| **Target URL** | `omiss[.]com` | Main bait site |
| **Hosting Provider** | `[REDACTED]` | High-risk provider with low cooperation policies |
| **Registrar** | `NameCheap, Inc.` | Use of Privacy Protection (WhoisGuard) |
| **IP Address** | `185.XXX.XXX.XX` | Shared server hosting 23 other suspicious instances |

### 🛡️ Indicators of Compromise (IoC)
* **Related Domains:** `omiss[.]net`, `omiss[.]org` [cite: immagine.png (9)]
* **Mail Server:** Missing SPF/DKIM records (clear spoofing indicators) [cite: immagine.png (9)]
* **Payment Gateway:** Forced redirection to `secure-checkout-gateway[.]ru` [cite: immagine.png (9)]

## 3. Investigative Methodology

### A. Certificate Transparency & Pivot Analysis
By monitoring SSL logs (via `crt.sh`), a pivot analysis was performed on the digital certificate.
* **Discovery:** The same certificate was issued simultaneously for 5 different domains, confirming a centralized attack rather than an isolated incident.

### B. SOCMINT Analysis
Analysis of social channels used for referral traffic:
* **Bot Detection:** Identified a network of approximately 1,200 automated profiles with synchronized posting patterns.
* **Geolocation:** Metadata residue and login traces localized the operational management in Eastern Europe, despite claiming an HQ in Northern Italy.

### C. Forensic Image Analysis
Verification of visual assets via `ExifTool` and Reverse Image Search:
* **Result:** Warehouse images presented as "authentic" were traced back to a German stock database from 2019. [cite: immagine.jpg (4)]
* **Manipulation:** Identified digital editing traces on logos using **ELA (Error Level Analysis)**. [cite: immagine.jpg (4)]

## 4. Conclusions
The investigation concluded with a comprehensive technical report for the client, including:
* Full list of **Indicators of Compromise (IoC)**. [cite: immagine.png (9)]
* **Chain of Custody** for digital evidence for legal purposes.
* Technical report submitted to registrars for the **Takedown** of the entire network. [cite: immagine.png (9)]

---
[🔙 Back to Portfolio](https://github.com/santivadaladev)
