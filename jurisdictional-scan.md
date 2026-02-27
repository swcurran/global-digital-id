# Digital ID Jurisdictional Scan

**Prepared for:** BC Government Digital Trust Initiative  
**Date:** 2026-02-27  
**Scope:** Global scan of digital ID issuance models, device strategies, and inclusion approaches

---

## Executive Summary

Digital ID systems have proliferated rapidly across the globe, with **37 of 50 major countries** now having implemented digital ID schemes. This scan examines:

1. **Device distribution models** — how many devices citizens can use to hold/present credentials
2. **Solutions for citizens without personal devices** — QR codes, kiosks, basic phones, biometric verification
3. **Multi-device and cloud-linked approaches** — emerging patterns beyond single-device storage

### Key Findings

- **IDs per person** — Most systems issue ONE credential per person (Aadhaar, NIN, Singpass). Some allow multiple: Estonia (card + Mobile ID + Smart ID), Sweden BankID (multiple devices), US mDL (via wallet sync). EUDI Wallet will support multiple credentials per person.
- **EU Digital Identity Wallet (2026)** — Mobile-first, multi-device capable, but member states must ensure inclusion
- **Mobile Driver's Licenses (US)** — 18 states by 2025, Apple/Google Wallet integration
- **Developing nations** — Often mandatory for service access; 73M+ Nigerians blocked from mobile networks for lacking digital ID
- **No-device solutions** — QR codes on plastic cards, biometric kiosks, government-issued basic phones exist but are not widespread

---

## Device Distribution Models

### Model Types

| Model | Description | Examples |
|-------|-------------|----------|
| **Single-device native** | Credential stored on one primary device | Most US mDL implementations |
| **Multi-device native** | Credentials sync across multiple devices (phone, tablet, wearable) | EUDI Wallet (planned), some Nordic systems |
| **Cloud-linked** | Central account that edge devices connect to | Singapore Singpass, India's DigiLocker |
| **Hybrid** | Combines local storage with cloud backup | Apple's ID cards in Wallet |

### Detailed Findings by Jurisdiction

---

## North America

### Canada

**Federal/Provincial Programs:**

- **BCID (British Columbia)** — In development, aligned with federal digital identity framework
- **Alberta** — Digital ID pilot programs
- **Ontario** — ServiceOntario digital services
- **Quebec** — Identité numérique Québec in development

**IDs per Person:** ONE credential per province. Canadians living in multiple provinces could have multiple provincial IDs.

**No-Device Solutions:** In-person Service BC/Ontario locations. No unified federal fallback.

**Note:** Canada lacks a unified national digital ID; provinces lead. Federal framework in development.

---

### United States — Subnational (State-Level)

**Mobile Driver's Licenses (mDL):**

As of 2025, **18 US states** have or are implementing digital IDs:

| State | Status | Platform |
|-------|--------|----------|
| Arizona | Active (2021) | Apple Wallet, Google Wallet |
| Colorado | Active | Apple Wallet, Google Wallet |
| Maryland | Active | Apple Wallet, Google Wallet |
| Georgia | Active | Apple Wallet, Google Wallet |
| Ohio | Active | Apple Wallet only |
| Louisiana | Active | Mobile-first |
| California | Active | Apple Wallet (Dec 2023) |
| Utah | Active | State app |
| Iowa | Active | State app |
| New York | Launching 2025 | TBD |
| New Jersey | Passed law 2025 | TBD |
| Tennessee | Coming | Apple Wallet |
| Virginia | Active | State app |
| Nevada | Active | TBD |
| Vermont | Active | TBD |
| Texas | In development | TBD |
| Florida | In development | TBD |
| Washington | In development | TBD |

**TSA Acceptance (as of 2024):** 11 states accepted at TSA checkpoints. REAL ID enforcement started May 2025.

**IDs per Person:** ONE mDL per person per state. Multiple devices can store same mDL via wallet sync.

**No-Device Solutions:** None at federal level; physical license + in-person DMV remain alternative.

---

### Mexico

**CURP (Clave Única de Registro de Población):**
- Unique ID number assigned to all Mexican residents
- Digital versions available through government apps
- Integration with immigration services

**Device Model:** Cloud-linked — credentials tied to centralized government accounts

---

## European Union

### EU Digital Identity Wallet (EUDI Wallet)

**Regulation:** eIDAS 2.0 (Regulation (EU) 2024/1183) — in force May 2024

**Timeline:**
- Implementing acts adopted: November 2024
- Member states must provide at least one wallet within **24 months** (by late 2026)

**Key Features:**
- Mobile-based identity wallet
- Store multiple credentials (ID, driver's license, health card, etc.)
- Cross-border interoperability across all 27 EU member states
- ISO/IEC 18013-5:2021 and ISO/IEC TS 18013-7:2024 standards
- User-controlled data sharing

**Device Model:** Designed for mobile-first, potential for multi-device sync through cloud backup

**No-Device Solutions:** Member states responsible for inclusion — no EU-wide mandate yet

**Privacy Score:** Higher (16/33) — GDPR provides strong baseline protections

---

### Individual EU Member States

#### Estonia

**System:** e-ID (mandatory since 2002)
- Over 99% of citizens hold digital ID
- ~70% regular usage

**Options:**
- Physical ID card with PKI chip
- Mobile ID (phone-based)
- Smart ID (smartphone app)

**Device Model:** Multi-channel — card, phone, tablet via Smart ID app

**e-Residency:** Digital ID for non-residents (109,000+ e-residents from 170 countries)

**No-Device Solutions:** Physical cards + in-person government service points

---

#### Sweden

**System:** BankID (de facto standard) + e-ID
- Over 8 million users
- Primarily mobile-based

**Device Model:** Multi-device — works on phone, tablet, computer

**No-Device Solutions:** Physical ID cards available, BankID on desktop

---

#### Denmark

**System:** MitID
- Replaced NemID in 2021
- App-based with code card fallback

**Device Model:** Primarily mobile app, with fallback options

---

#### Germany

**System:** Online-Ausweisfunktion (eID) — embedded in new ID cards
- Electronic ID available since 2010
- EUDI Wallet integration coming 2026

**Device Model:** Physical card + smartphone (with NFC reading)

---

#### Greece

**System:** Digital ID in government wallet app
- Stores regular ID with QR code
- Can scan other IDs' QR codes for verification

---

## Asia Pacific

### Singapore — Singpass

**Scale:** 5M+ users, 2,700+ services, 800+ organizations, 41M+ monthly logins

**Device Model:** Mobile app with multiple authentication methods:
- Facial recognition
- Fingerprint scan
- QR code login
- 2FA/SMS OTP

**Cloud-linked:** Yes — centralized authentication links to government services via MyInfo

**No-Device Solutions:**
- QR codes for those without smartphones
- In-person service centres
- Facial recognition at kiosks

**Privacy Score:** 16/33 (relatively lower due to data sharing with third parties)

---

### India — Aadhaar

**Scale:** 1.3+ billion enrolled — world's largest digital ID system

**Device Model:** 
- Unique 12-digit number linked to biometrics (fingerprints, iris)
- Not device-specific — authentication via UIDAI infrastructure
- eKYC allows real-time verification without physical document
- DigiLocker provides cloud-based document storage

**Key Stats (March 2025):**
- 446M+ eKYC transactions in single month
- 23.5B+ cumulative transactions

**No-Device Solutions:**
- OTP fallback (SMS/email)
- In-person enrollment centres
- Aadhaar-enabled banking correspondents (banking guides in rural areas)
- Face authentication (rolled out as alternative to fingerprint)

**Privacy Score:** Lower — centralized biometric database, concerns about surveillance. Virtual ID (VID) introduced for privacy.

---

### Australia

**System:** myGov ID (federal), various state programs

**Device Model:** Mobile app-based, cloud-linked

**No-Device Solutions:** myGov in-person service centres, Medicare cards

---

### Malaysia

**System:** MyDigital ID

**Device Model:** Mobile app — if phone lost/damaged, must revoke certificate at kiosk before re-registering new device

**No-Device Solutions:** Government kiosks for re-registration

---

### Japan

**System:** My Number Card (individual number)
- Digital version in development
- Integration with smartphone wallets

**Device Model:** Physical card + mobile app integration coming

---

### China

**System:** National Online Identity Authentication (launched July 2025)

**Device Model:** Mobile app + centralized database

**Key Features:**
- "Web number" and "web certificate" for verification
- Facial recognition required
- Voluntary registration but encouraged for public/private services
- WeChat, Xiaohongshu, Taobao already integrated

**No-Device Solutions:** Physical ID card alternative exists

**Privacy Score:** 12.5/33 (lowest) — centralized data, limited privacy law, data disclosure overrides

---

## Middle East

### UAE

**System:** UAE Pass

**Scale:** 12,000+ government and private sector services

**Device Model:** Mobile app (mandatory for some services)

**Privacy Score:** 15/33 — mandatory for certain government services

---

## Africa

### Nigeria — NIN (National Identification Number)

**Scale:** 95M+ enrolled (target: 148M by 2024)

**Device Model:** Mobile app (NINAuth), centralized database

**Critical Issue — No-Device Exclusion:**
- **73 million Nigerians** lost partial mobile network access for not having NIN
- SIM registration requires NIN
- Legislation makes NIN compulsory for healthcare, education, banking

**Privacy Score:** 14/33 — centralized database, mandatory

---

### Ghana

**System:** Ghana Card

**No-Device Solutions:**
- SIM registration requires Ghana Card
- In-person enrollment

---

### Kenya

**System:** eCitizen platform, National ID integration

**No-Device Solutions:**
- SIM registration requires National ID
- eCitizen accessible via any browser
- Huduma Centres (one-stop government service centres)

---

### Other African Countries

Countries with national IDs with electronic components:
- Algeria, Angola, Cameroon, Egypt, Lesotho, Mauritius, Morocco, Senegal, Seychelles, Rwanda, South Africa, Tanzania, Uganda, Zimbabwe

---

## Latin America

### Brazil

**System:** RG digital (driver's license with QR code, photo, biometrics)
- Digital versions via government app since 2017

**Device Model:** Physical card + mobile app

---

## Solutions for Citizens Without Personal Devices

### Overview of Approaches

| Approach | Countries Using | Notes |
|----------|-----------------|-------|
| **QR codes on plastic cards** | Greece, Brazil (driver's license), some US states | Static or dynamic QR for verification |
| **Government-issued basic phones** | Not widely adopted | Some pilot programs in developing nations |
| **Biometric kiosks** | India (Aadhaar), some African nations | In-person verification points |
| **Paper-based with digital verification** | Various | NIN slip in Nigeria, Aadhaar PVC card |
| **Shared device programs** | India (banking correspondents), Kenya (Huduma) | Community access points |
| **OTP/face authentication fallback** | India, various | SMS or facial recognition alternatives |

### Key Observations

1. **Most digital ID systems assume smartphone/device ownership** — exclusion is a significant challenge
2. **Developing nations often mandate ID for essential services** — creating pressure to obtain ID even without devices
3. **QR codes on cards** — simplest no-device solution, but limited functionality (mostly verification, not authentication)
4. **Biometric kiosks** — India has the most extensive network (100K+ Aadhaar enrollment centres)
5. **Community-based access** — India's banking correspondents and Kenya's Huduma centres provide models

---

## Multi-Device and Wearable Approaches

### Current State

- **Limited multi-device support** — Most systems are single-device or account-based
- **Cloud-linked is more common** — Singpass, DigiLocker, EUDI Wallet design
- **Wearable integration** — Not widely implemented; Apple Watch can store some IDs (US states supporting Apple Wallet)

### Emerging Trends

1. **EUDI Wallet** — Will support credential presentation from multiple devices
2. **Cloud backup/sync** — Google Wallet, Apple Wallet enable backup and restore
3. **Cross-device authentication** — BankID (Sweden), MitID (Denmark) work across devices
4. **IoT/connected device presentation** — ISO 18013-7 (mDL) enables device-to-device communication

---

## Gap Analysis for BC

### Questions for Further Investigation

1. **Inclusion strategy** — What fallback mechanisms will BC offer for citizens without smartphones?
2. **Multi-device** — Will BCID support multiple devices per citizen? Cloud backup?
3. **Interoperability** — Will BCID work with EUDI Wallet? US state mDLs?
4. **Offline capability** — Does BC need offline verification for remote/underserved areas?
5. **Privacy framework** — How does BCID compare to EU/GDPR standards?

---

## Sources

- Comparitech — Digital IDs: 50 countries ranked (November 2025)
- Identity.com — 7 Countries Implementing Digital ID Systems (December 2025)
- EU Digital Identity Wallet — European Commission
- TSA — Digital ID Participating States
- UIDAI — Aadhaar statistics (2025)
- e-Estonia — e-Residency data
- Regula Forensics — Digital ID Overview by Country (December 2025)
- World Bank — ID4D Global Dataset

---

*This document will be updated as new information becomes available.*
