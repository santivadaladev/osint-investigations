# OSINT CASE STUDY N°002
# RUSSIA–UKRAINE WAR (2022–PRESENT)

> **Classification:** Public  
> **Dossier:** N° 002  
> **Primary Sources:** ISW · Oryx · DeepState · BBC/Mediazona · Bellingcat · CSIS · OHCHR · Meduza  
> **Last Updated:** May 2026

---

## TABLE OF CONTENTS

1. [Conflict Overview](#1-conflict-overview)
2. [Causes and Origins](#2-causes-and-origins)
3. [OSINT Methodology and Key Actors](#3-osint-methodology-and-key-actors)
4. [Global Data](#4-global-data)
5. [Mobilisation and Conscription](#5-mobilisation-and-conscription)
6. [Named Casualty Identification](#6-named-casualty-identification)
7. [Ethical Notes and OSINT Limitations](#7-ethical-notes-and-osint-limitations)

---

## 1. CONFLICT OVERVIEW

| Data Point | Value |
|------------|-------|
| Start of full-scale invasion | 24 February 2022 |
| Duration | 3+ years (ongoing) |
| Ukrainian territory under Russian occupation (Dec. 2025) | ~116,000 km² · ~19.2% of the country |
| Estimated total casualties (killed + wounded, both sides) | 1.4 million+ |

The conflict is rooted in the collapse of the USSR (1991) and the identity, geopolitical and linguistic tensions between Russia and Ukraine. The crisis accelerated with Euromaidan (2013–14), the illegal annexation of Crimea and the Donbas war (2014–2021, ~14,200 deaths). On 24 February 2022, Russia launched a full-scale invasion under the declared objectives of "denazification" and "demilitarisation" of Ukraine.

The failure of the advance on Kyiv (April 2022) transformed the conflict into an **attritional war of attrition** unprecedented in Europe since World War II.

### The Role of OSINT

The Russia–Ukraine war has become the **first large-scale conflict of the social media era**, in which Open Source Intelligence has played a decisive role:

- Real-time tracking of equipment losses
- Nominal identification of Russian casualties
- Documentation of war crimes
- Geolocation of strikes and bombardments
- Predicting the invasion hours before it began (Google Maps traffic data)

---

## 2. CAUSES AND ORIGINS

### 1991–2013 — Post-Soviet Legacy

The dissolution of the USSR left unresolved borders and identities. Independent Ukraine harboured a large Russian-speaking minority in its eastern and southern regions. Russia applied sustained pressure to maintain its sphere of influence through the CIS and preferential energy agreements.

### 2013–2014 — Euromaidan and the Annexation of Crimea

President Yanukovych suspended the EU Association Agreement, triggering mass protests on Kyiv's Maidan square. Following his flight from the country, Russia illegally annexed Crimea (March 2014) and backed separatist movements in the Donbas. The Donbas conflict (2014–2021) caused between 14,200 and 14,400 deaths, of which at least 3,400 were civilians (OHCHR).

### 2014–2021 — Donbas War and the Minsk Agreements

Low-intensity conflict in the Donetsk and Luhansk regions. The Minsk I (2014) and Minsk II (2015) agreements were never fully implemented. Ukraine accelerated its integration process toward NATO and the EU. Moscow interpreted this trajectory as an existential security threat.

### 2021 — Troop Build-up and Ultimatum

Russia massed over 100,000 troops along the Ukrainian border. In December 2021, Putin delivered a written ultimatum to the US and NATO demanding formal guarantees against further eastward expansion of the Alliance. The West refused the demands.

### 24 February 2022 — Full-Scale Invasion

Putin declared the start of a "special military operation" citing denazification and protection of Russian-speaking populations. Russian forces launched simultaneous attacks from the North (through Belarus), the East (Donbas) and the South (Crimea). The advance on Kyiv collapsed by April 2022.

### 2022–2026 — Prolonged War of Attrition

Following the failure of the initial objectives, the conflict settled into a grinding trench war. Ukraine's autumn 2022 counteroffensive recaptured Kharkiv and Kherson. From 2023 onward, the front largely stalled with slow Russian advances in eastern Donetsk.

> **OSINT Methodological Note:** The causes of the conflict are subject to deep narrative contestation. Russian sources emphasise NATO expansion and the "protection of Russian speakers." Ukrainian and Western sources stress imperialist aggression and violation of sovereignty. OSINT analysis focuses on verifiable facts (troop movements, losses, territory) while keeping structural causation analysis separate.

---

## 3. OSINT METHODOLOGY AND KEY ACTORS

### Principal Organisations

| Organisation | Country | Speciality | Key Contribution |
|--------------|---------|------------|-----------------|
| **Bellingcat** | 🇳🇱 Netherlands | Geolocation, war crimes | Interactive maps of civilian targets struck; authentication of war crimes evidence (Bucha). Banned in Russia July 2022. |
| **Oryx** | 🌐 International | Equipment losses with visual evidence | Systematic vehicle-by-vehicle count of confirmed losses using photo/video evidence from social media. |
| **DeepState (UKR)** | 🇺🇦 Ukraine | Real-time front-line map | Continuous front-line updates; ~116,000 km² of occupied territory mapped as of December 2025. |
| **ISW** | 🇺🇸 USA | Daily operational analysis | Daily field manoeuvre reports; strategic forecasts; analysis of Russian territorial gains. |
| **BBC / Mediazona** | 🇬🇧🇷🇺 UK–Russia | Nominal ID of Russian casualties | Database of ~96,000 Russian soldiers identified by name (February 2025). |
| **Kharon (iStories)** | 🇷🇺 Russia (independent) | Named casualty registry | 104,000 Russian deaths identified from open sources, including DNR/LNR fighters. |
| **Middlebury MIIS** | 🇺🇸 USA (academic) | Pre-invasion analysis | Detected an anomalous traffic jam on Google Maps near the Ukrainian border hours before the invasion. |

### OSINT Techniques Employed

**Geolocation**
Systematic comparison of social media images and videos with Google Maps, Google Earth and Street View to pinpoint the exact location of strikes, war crimes and troop movements.

**Social SIGINT**
Analysis of posts published on Russian platforms (VK, Telegram) by soldiers and their families, which inadvertently revealed positions, losses and operational conditions.

**Probate Registry Analysis**
Tracking of inheritance and property transfers to estimate the number of deaths not officially declared by Russia. Meduza and Mediazona used this method to estimate ~352,000 Russian male deaths (ages 18–59) through the end of 2025.

**Facial Recognition**
Used by some OSINT organisations to attempt to identify those responsible for war crimes, notably in the Bucha massacre investigation.

**Commercial Satellite Imagery**
Monitoring of troop movements, infrastructure destruction and port activity. Companies such as Maxar Technologies provided imagery that proved decisive in tracking Russian deployments.

**Traffic Analysis**
The most emblematic case: the Middlebury Institute detected an anomalous traffic jam via Google Maps on a Russian road toward the Ukrainian border on the night of 23–24 February 2022, anticipating the invasion by approximately one hour.

---

## 4. GLOBAL DATA

> ⚠ **Warning:** Casualty data are contested. Russian figures are classified. Estimates vary significantly across sources and must be treated as approximations.

### 4.1 Russian Military Casualties

| Indicator | Estimate | Source |
|-----------|----------|--------|
| Named deaths confirmed by OSINT | ~96,000 | BBC/Mediazona, Feb. 2025 |
| Estimated total deaths | ~219,000–250,000 | Mediazona / CSIS, 2025 |
| Wounded | ~700,000+ | CSIS, UK MoD, Jun. 2025 |
| Officially listed missing | 84,568 | Russia Matters |
| **Total casualties** | **~950,000–1,000,000+** | CSIS / UK MoD / ISW |
| Confirmed officer deaths | 7,094 (as of 9 May 2026) | Mediazona |
| % of Russian men aged 20–50 killed or seriously wounded | ~2% | Meduza / Mediazona |

**Chronological estimates (Russia):**
- 600,000 killed + wounded — Trump, December 2024
- ~1,000,000 killed — Trump, January 2025
- 750,000+ — US DNI / intelligence community, March 2025
- 950,000+ (250,000 killed) — CSIS, June 2025
- 1,000,000+ (250,000 killed) — UK MoD, June 2025
- 352,000 deaths (men aged 18–59) — Meduza / Mediazona estimate, 2025

### 4.2 Ukrainian Military and Civilian Casualties

| Indicator | Estimate | Source |
|-----------|----------|--------|
| Soldiers killed | ~46,000+ | Zelensky, Feb. 2025 |
| Soldiers wounded | ~380,000 | Zelensky, Feb. 2025 |
| Total killed + wounded (range) | 60,000–400,000 | The Economist, Nov. 2024 |
| Missing | 35,000 | Russia Matters |
| Civilians killed | ~13,883 | OHCHR, 2022–2026 |
| Internally displaced persons | ~5 million | UNHCR, 2025 |
| Refugees abroad | ~6–8 million | UNHCR, 2024 |

### 4.3 Equipment Losses (Source: Oryx — visually confirmed only)

| Category | Russia | Ukraine |
|----------|--------|---------|
| Total vehicles lost | 23,715+ | 10,869+ |
| Tanks / armoured vehicles | 13,742 | 5,423 |
| Aircraft | 353 | 192 |

### 4.4 Territorial Control (DeepState OSINT, December 2025)

| Data Point | Value |
|------------|-------|
| Russian-occupied Ukrainian territory | ~116,000 km² (~19.2%) |
| Geographic equivalent | US state of Pennsylvania |
| Russian gains since 24/2/2022 (incl. Crimea) | +~75,000 km² |
| Average rate of Russian advance (2025) | 176 sq mi/month (ISW) |

### 4.5 Destruction of Ukrainian Infrastructure

| Infrastructure | Damage | Date of Estimate |
|----------------|--------|-----------------|
| Electricity generating capacity destroyed / occupied | 64% (36 of 56 GW) | 2024 |
| Thermal power capacity destroyed | ~90% | May 2025 |
| Hydropower installations damaged | 50% (40% destroyed) | May 2025 |
| Remaining electricity capacity | ~1/3 of pre-invasion level | Autumn 2025 |
| Russian oil refining capacity offline (Ukrainian drone strikes) | ~40% | October 2025 |
| Ukraine fiscal deficit 2024 | 20.4% of GDP (excl. grants) | World Bank |
| Ukrainian gas production destroyed | ~60% | October 2025 |

---

## 5. MOBILISATION AND CONSCRIPTION

### Russian Partial Mobilisation — 21 September 2022

Putin announced a partial mobilisation calling up 300,000 reservists. The civilian response was immediate: approximately **800,000 Russians left the country** for political and economic reasons (0.6% of the population). Protests erupted in 38 Russian cities, with thousands of arrests. The measure triggered a recruitment and demographic crisis that Russia sought to offset through alternative methods.

### Prison Recruitment — Wagner PMC (Summer 2022 – 2023)

Yevgeny Prigozhin recruited directly in Russian prisons. Up to 50,000 former convicts were enlisted and deployed in frontal assaults on Bakhmut. High mortality was intrinsic to the model: by March 2023, prisoners had become the **largest single category of Russian casualties**. After the fall of Bakhmut, mass prison recruitment gradually ceased.

### Commercial Volunteers (2023–2026)

As prison recruitment waned and no new formal mobilisation was announced, Russia dramatically increased financial bonuses for voluntary enlistment. "Commercial volunteers" became the **largest category of Russian casualties** from September 2024 onward. The average age of the fallen increased: 34% of fallen volunteers were between 42 and 50 years old.

### Ukrainian Mobilisation Law — April 2024

Ukraine lowered the minimum conscription age from 27 to 25 with a controversial mandatory mobilisation law. Difficulties in recruiting new cohorts remained significant. Zelensky updated casualty figures in February 2025: 46,000 soldiers killed and 380,000 wounded, with approximately 50% of the wounded having returned to active duty.

### Demographic Profile of Russian Casualties by Year

| Year | Predominant Age Group | Primary Category |
|------|-----------------------|-----------------|
| 2022 | 20–29 years (41%) | Regular professional army |
| 2023 | 30–39 years (38%) | Mobilised + Wagner / prisoners |
| 2024 | 42–50 years (34% of volunteers) | Commercial volunteers |
| Mobilised (overall) | 30–41 years (52%) | Older reservists |
| Prisoners (overall) | 30–41 years (48%) | Prison recruits |

---

## 6. NAMED CASUALTY IDENTIFICATION

One of the most significant OSINT applications in this conflict has been the construction of **named databases of fallen Russian soldiers**. This is made possible by the relative openness of Russian social media (VK), local obituaries, probate registries and online memorial pages.

### Primary Databases

**BBC / Mediazona**
- Soldiers identified by name: **~96,000** (February 2025)
- Method: obituaries, social media (VK), civil registries, local official sources
- Source: en.zona.media / bbc.com/russian

**Kharon Project (iStories)**
- Deaths identified: **~104,000**
- Includes DNR/LNR fighters (Donetsk and Luhansk), with 39,600 cases with known age
- Enables detailed demographic analysis by year and recruitment category
- Source: istories.media

**Meduza / Total Estimate**
- Estimate via probate registry: **~352,000 deaths** (men aged 18–59, through 2025)
- Method: analysis of anomalous male deaths recorded in the Russian probate registry since 24/2/2022
- Source: meduza.io

> OSINT named databases are estimated to capture only **25–30% of actual Russian deaths**.

### Confirmed Russian Officers Killed (Selection from Open Sources)

As of 9 May 2026, **7,094 officers** have been confirmed killed (Mediazona). The share of officers among total casualties has steadily declined from the initial ~10% (when the professional contract army dominated) as mobilised soldiers and volunteers became the primary component.

| Name | Rank / Unit | Date | Notes |
|------|-------------|------|-------|
| Andrei Sukhovetsky | Maj. Gen. · 41st Army | First weeks of war, 2022 | First confirmed general killed |
| Vladimir Frolov | Maj. Gen. · 8th Army | April 2022 | Among the first high-ranking losses |
| Roman Kutuzov | Maj. Gen. | June 2022 | Killed in attack on troop formation |
| Igor Kirillov | Lt. Gen. · NBC Protection Troops | December 2024 | Killed by bomb in Moscow |
| Yaroslav Moskalik | Lt. Gen. · General Staff | April 2025 | Killed by car bomb, Moscow suburb |
| Fanil Sarvarov | Lt. Gen. · Operational Training Directorate | December 2025 | Killed by car bomb in Moscow |
| Mikhail Gudkov | Adm. · Deputy Commander-in-Chief of the Navy | July 2025 | Killed in strike on 155th NI Brigade HQ |

---

## 7. ETHICAL NOTES AND OSINT LIMITATIONS

### Quantitative Limitations

- Russian casualty figures are classified and systematically understated by the Moscow government
- OSINT named databases cover an estimated 25–30% of actual deaths
- Ukrainian figures are classified for national security reasons
- Estimates from different actors (Trump, ISW, CSIS, UK MoD) vary by as much as 50–100%
- OHCHR civilian casualty figures are individually verified but represent a confirmed lower bound

### Ethical Issues

The publication of named data on the fallen is a matter of ongoing debate. On one hand, it guarantees **transparency** against the official Russian narrative that minimises losses and allows families to learn the fate of their relatives. On the other, the dissemination of personal data and images of bodies on social media has raised significant ethical concerns.

Organisations such as BBC/Mediazona operate under multi-source verification standards for every name included. The use of facial recognition technology to identify potential war crimes perpetrators raises further legal and privacy questions.

### Risk of Manipulation

Both sides actively produce and disseminate disinformation. OSINT reduces but does not eliminate the risk of being deceived by manipulated material, decontextualised videos or fabricated data. Cross-verification across independent sources remains the fundamental methodology.

---

## PRIMARY SOURCES

- Institute for the Study of War (ISW) — isw.is
- Oryx — oryxspioenkop.com
- DeepState Ukraine — map.deepstatemap.live
- BBC / Mediazona — en.zona.media
- Bellingcat — bellingcat.com
- CSIS (Center for Strategic & International Studies) — csis.org
- Russia Matters / Belfer Center Harvard — russiamatters.org
- OHCHR (UN Human Rights Monitoring Mission in Ukraine) — ohchr.org
- Meduza — meduza.io
- Kharon / iStories — istories.media
- The Economist — economist.com
- Wikipedia: *Casualties of the Russo-Ukrainian War* / *Open-source intelligence in the Russian invasion of Ukraine*

---

*OSINT Dossier N°002 · Russia–Ukraine Conflict · Updated May 2026*
