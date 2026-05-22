# ⚡ OPERATION CERBERUS-LINK (CASE OSC-2026-02)
> **CLASSIFICATION:** HIGHLY CONFIDENTIAL // THREAT INTELLIGENCE OPERATIVE REPORT
> **TARGET PROFILE:** Valtteri K. (Helsinki, Finland) // Aliases: `[REDACTED]` / `[REDACTED]`
> **STATUS:** 🔴 CLOSED (TARGET DEFINITIVELY IDENTIFIED)
> **METHODOLOGY:** MULTI-PLATFORM PIVOT ANALYSIS & OPSEC EXPLOITATION

---

## 1. Executive Summary
This intelligence report documents the operational activities regarding case **OSC-2026-02**. The primary objective of this investigation was to identify the operator behind the infrastructure and source code repository known as **"Project-Cerberus"**. Through structured passive analysis and the strategic exploitation of catastrophic OPSEC (Operational Security) failures committed by the target, the threat actor's true identity has been definitively mapped to **Valtteri K.**, residing in Helsinki, Finland.

---

## 2. Target Profile Summary

| Investigative Attribute | Extracted / Identified Data | Technical Context // Notes |
| :--- | :--- | :--- |
| **True Name** | Valtteri K. | Identified via Google API enumeration |
| **Primary Location** | Helsinki, Finland | Timezone alignment (EET/UTC+2) & physical footprint |
| **Active Telegram** | `@[REDACTED]` | Permanent User ID: `558392011` |
| **Development Email** | `[REDACTED]` | Extracted from GitHub historical commit cache |
| **Legacy Email** | `[REDACTED]` | Retrieved from historical underground forum leak |
| **Infrastructure Node** | `HEL-01` | Public IPFS Node tied directly to the target |

---

## 3. Investigation Intelligence Graph & Pivot Timeline

```text
[Legacy Forum Leak] ──> Nickname: [REDACTED] & [REDACTED]
                             │
                             ▼ (GitHub Cache Inspection)
                      [Project-Cerberus] ──> Email: [REDACTED]
                                                   │
                                                   ▼ (GHunt / API Email Pivoting)
                                            [Google Account] ──> True Name: "Valtteri K."
                                                   │
                                                   ▼ (Google Maps Passive Reviews)
                                            Location: Helsinki (Kamppi/Pasila)
                                                   │
                                                   ▼ (OPSEC Leak: IPFS Config History)
                                            [Keybase Public Key] & [Telegram History Log]
                                                   │
                                                   ▼ (Persistent UID Tracking)
                                            New Telegram Account: @[REDACTED]
                                                   │
                                                   ▼ (Terminal Prompt Match)
                                            Host Target Matching: [REDACTED]@hel-01

4. Chronological Analysis & Findings
Phase 1: Initial Reconnaissance & Cache Retrieval

    The Ingestion Point: A historical credential leak from a defunct underground discussion forum exposed the alias [REDACTED] associated with a legacy ProtonMail address.

    GitHub Cache Pivoting: Target code footprinting on GitHub revealed a deleted repository named Project-Cerberus. A deep metadata inspection of the historical git commits cached on the platform exposed a secondary, active development email address: [REDACTED].

Phase 2: Social Media Intelligence (SOCMINT) & Geolocation

    Google Account Enumeration: Utilizing manual API interrogation techniques (via GHunt/Epieos methodologies) against the development Gmail string, the target's true name string was extracted: "Valtteri K.".

    Geographic Correlation: Public OSINT scrapers mapping the target's unique Google ID revealed a consistent pattern of physical activity and point-of-interest reviews located in central Helsinki, Finland, specifically within the Kamppi Center and Pasila districts.

    Timezone Verification: An operational review of an alternative microblogging platform (Mastodon) captured a post by the target stating: "Still 2 hours of calls with London clients, it's already 11 PM here". Cross-referencing the +2 hour delta from London (UTC+0) perfectly validates Helsinki winter time (EET, Eastern European Time / UTC+2).

Phase 3: Exploiting OPSEC Failures

    The IPFS Leak: While publishing a hardware benchmarking thread on a local IT retail forum, the target attached a link pointing to a public IPFS node (HEL-01). Archive history captured a peer response warning the target that their exposed config.json file inadvertently leaked their public Keybase identity and legacy Telegram handle (@[REDACTED]).

    Persistent ID Recovery: Although the target purged the @[REDACTED] handle to avoid attribution, historical threat intelligence database logs mapped the deleted handle to a permanent, unchangeable Telegram User ID: 558392011.

    Reverse UID Lookup: Continuous passive monitoring of UID 558392011 captured a handle update, exposing the target's newly created, active Telegram identity: @[REDACTED].

Phase 4: The Smoking Gun (Definitive Attribution)

The target published a screenshot on their Mastodon account (cryptographically verified via their Keybase public key) complaining about a local code compilation error. A close inspection of the underlying Linux terminal prompt in the image exposed the following system string:
[REDACTED]@hel-01:~/projects/project-cerberus$

This specific data point closes the investigation with absolute certainty, matching:

    The local system username ([REDACTED]) to the newly discovered active Telegram identity.

    The local hostname (hel-01) to the leaked public IPFS node network footprint.

    The working directory directly to the target repository (project-cerberus).

5. Tactics, Techniques, and Procedures (Manual Kali Linux)

    Email Enumeration & Profiling: GHunt, Holehe, Epieos API integration.

    Historical OSINT Operations: Google Cache engine, Wayback Machine, Telegram Core API Logs.

    Intelligence Synthesis: Manual structured Markdown link analysis.

6. Recommendations & Next Steps

    Passive Signals Intelligence: Deploy a passive, non-intrusive logger on public infosec Telegram channels indexed by UID 558392011 to monitor future infrastructure discussions.

    Repository Monitoring: Configure automated GitHub dork alerts to intercept any newly pushed repositories matching the specific structural code signatures or comments unique to the Project-Cerberus codebase.

REPORT GENERATED VIA PRIVACY SYSTEM • OPERATOR: [REDACTED] // CASE OSC-2026-02