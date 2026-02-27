# Digital ID Jurisdictional Scan - Deep Dive

**Prepared for:** BC Government Digital Trust Initiative  
**Date:** 2026-02-27  
**Scope:** Global scan of digital ID systems with technology specifications

---

## Executive Summary

Digital ID systems have proliferated across the globe with significant variation in:
- **Technology stack** (PKI, biometrics, blockchain, cloud-native)
- **Issuance model** (single credential, multi-device, cloud-linked)
- **Governance** (government-led, bank-led, public-private partnerships)
- **Inclusion approaches** (no-device solutions, offline fallback)

This scan provides deep technical detail for 20+ national systems and 30+ subnational jurisdictions.

---

## Technology Definitions

| Technology | Description | Examples |
|------------|-------------|----------|
| **PKI (Public Key Infrastructure)** | Cryptographic certificates stored on secure elements | Estonia e-ID, German eID, Finnish Trust Network |
| **Biometric Authentication** | Fingerprint, iris, face recognition for verification | India Aadhaar, Nigeria NIN, Israel |
| **Mobile-Based** | Credentials stored in mobile apps | US mDL, Korean Mobile ID, Swedish BankID |
| **Cloud-Native** | Central identity provider with API access | Singapore Singpass, Kenya eCitizen, Australia myGov |
| **Wallet Architecture** | User controls credentials, presents on demand | EUDI Wallet (pending), Apple/Google Wallet mDL |
| **FIDO2/WebAuthn** | Passwordless authentication standard | Supported by EUDI, various EU member states |

---

## National Systems - Detailed

### 🇪🇺 European Union - EUDI Wallet (Specification)

**Technology:** Wallet architecture based on ISO/IEC 18013-5 (mDL) + SD-JWT (Selective Disclosure JWT)  
**Specification:** eIDAS 2.0 Regulation (2024/1183)  
**Target Launch:** End 2026 (mandatory for all 27 member states)  
**Official Sources:**
- European Commission: https://commission.europa.eu/topics/digital-economy-and-society/european-digital-identity_en
- EUDI Wallet Overview: https://github.com/eu-digital-identity-wallet/
- eIDAS 2.0: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1183

**Technical Details:**
- User-controlled wallet (not government-issued)
- QES (Qualified Electronic Signature) support
- PID (Personal Identification Data) credential
- Cross-border interoperability via EUDI Node
- Wallet ID (WID) specification in development

---

### 🇬🇧 United Kingdom - BritCard (Specification)

**Technology:** Centralized digital identity with attribute sharing  
**Status:** Announced September 2025, mandatory for right-to-work by 2029  
**Official Sources:**
- UK Digital Identity Framework: https://www.gov.uk/government/collections/uk-digital-identity-and-attributes-trust-framework
- DCMS Policy Paper: https://www.gov.uk/government/publications/uk-digital-identity-and-attributes-trust-framework-better-for-business
- UK Statistics: https://www.ons.gov.uk/

**Technical Details:**
- Voluntary framework but mandatory for certain services
- Trust framework with accredited identity providers
- Data privacy emphasis (user control over attributes)
- Integration with GOV.UK Verify (now deprecated)

---

### 🇮🇳 India - Aadhaar (Production)

**Technology:** Biometric-based centralized identity with OTP fallback  
**Enrolled:** 1.3+ billion residents (world's largest)  
**Monthly Transactions:** 446M+ eKYC  
**Official Sources:**
- UIDAI: https://uidai.gov.in/
- Aadhaar Technology: https://uidai.gov.in/aadhaar-technology
- DigiLocker: https://digitallocker.gov.in/

**Technical Details:**
- 12-digit unique Aadhaar Number linked to biometrics (fingerprints, iris)
- OTP via SMS/email as fallback for those without biometrics
- Face authentication introduced as alternative
- eKYC (electronic Know Your Customer) API for service providers
- Virtual ID (VID) for privacy protection
- 100K+ enrollment centres nationwide
- Banking correspondents in rural areas (BC - Banking Correspondents)

---

### 🇸🇬 Singapore - Singpass (Production)

**Technology:** Cloud-native centralized identity with MyInfo for data sharing  
**Users:** 5M+ (entire adult population)  
**Services:** 2,700+ government and private sector  
**Official Sources:**
- Singpass: https://www.singpass.gov.sg/
- GovTech Singapore: https://www.tech.gov.sg/products-and-services/for-citizens/digital-services/singpass/
- Developer Portal: https://www.developer.tech.gov.sg/products/categories/digital-identity/singpass/
- sgID: https://id.gov.sg/ (for private sector)

**Technical Details:**
- Cloud-based identity with centralized authentication
- Multi-factor: Password + SMS/email OTP + biometrics (face/fingerprint)
- MyInfo: Pre-fills forms with government-held data (consent-based)
- Digital IC (Identity Card) in app for government counter verification
- sgID for private sector verification
- QR code login for feature phones

---

### 🇰🇷 South Korea - Mobile Digital ID (Production)

**Technology:** Mobile-based with certificate authentication  
**Launch:** March 2025 (nationwide)  
**Official Sources:**
- Government Portal: https://www.gov.kr/
- Ministry of the Interior and Safety: https://www.mois.go.kr/
- Korea Internet & Security Agency (KISA): https://kisa.or.kr/

**Technical Details:**
- Digital residence cards on smartphone
- Certificate-based authentication (public key infrastructure)
- **Note:** Not yet compliant with ISO 18013-5 or SD-JWT standards
- Android and iOS support
- Government-issued certificates

---

### 🇹🇼 Taiwan - Digital Wallet (Specification)

**Technology:** Wallet architecture (National Digital Wallet)  
**Target:** End 2025  
**Official Sources:**
- Executive Yuan: https://www.ey.gov.tw/
- Digital Development Agency: https://dda.gov.tw/

**Technical Details:**
- Will hold digital ID, certificates, driver's license, health card
- Integration with existing government systems
- Mobile-first approach

---

### 🇪🇪 Estonia - e-ID (Production)

**Technology:** PKI-based with multiple credential options  
**Coverage:** 99%+ of adult population  
**Official Sources:**
- e-Estonia: https://e-estonia.com/
- Police and Border Guard Board: https://www.politsei.ee/
- e-Residency: https://e-resident.gov.ee/

**Technical Details:**
- **Three credential types:**
  1. ID card (physical, with PKI chip)
  2. Mobile ID (SIM-based, works on any phone)
  3. Smart ID (app-based, works on any smartphone)
- X-Road (secure data exchange layer)
- DigiDoc (digital signature container)
- e-Residency: Digital ID for non-citizens (109K+ e-residents)

---

### 🇸🇪 Sweden - BankID (Production)

**Technology:** Bank-issued PKI certificates, soft tokens  
**Users:** 8M+ (population ~10M)  
**Official Sources:**
- BankID: https://www.bankid.com/
- BankID for Developers: https://www.bankid.com/en
- Swedish e-Identification: https://www.eidentitet.se/

**Technical Details:**
- Private sector led (major Swedish banks)
- BankID on file (computer), Mobile BankID (phone), BankID card
- Cryptographic keys stored in mobile app
- Works across devices (multi-device)
- Not government-issued but government-backed
- Cross-platform (iOS, Android, desktop)

---

### 🇩🇪 Germany - Online-Ausweisfunktion (Production)

**Technology:** NFC-enabled ID card with eID function  
**Since:** 2010  
**EUDI Integration:** Coming 2026  
**Official Sources:**
- BSI (Federal Office for Information Security): https://www.bsi.bund.de/EN/Themen/Oeffentliche-Verwaltung/Elektronische-Identitaeten/Online-Ausweisfunktion/online-ausweisfunktion_node.html
- Personalausweis Portal: https://www.personalausweisportal.de/

**Technical Details:**
- eID function embedded in new ID cards (since 2010)
- NFC reading via smartphone (Android with NFC, iOS 13+)
- Optional (not activated by default)
- Browser-based authentication via AusweisApp2
- PIN required for identification

---

### 🇨🇳 China - National Online Identity (Production)

**Technology:** Centralized with facial recognition  
**Launch:** July 2025  
**Official Sources:**
- Government Portal: https://www.gov.cn/
- Ministry of Public Security: https://www.mps.gov.cn/

**Technical Details:**
- One online ID per citizen linked to national ID card
- Facial recognition required for activation
- WeChat integration for convenience
- Centralized database
- Voluntary but encouraged for services

---

### 🇳🇬 Nigeria - NIN (Production)

**Technology:** Biometric central database  
**Enrolled:** 95M+  
**Critical Issue:** 73M+ blocked from mobile networks for lacking NIN  
**Official Sources:**
- NIMC: https://nimc.gov.ng/
- NIN Verification: https://verification.nimc.gov.ng/

**Technical Details:**
- One NIN per citizen
- Biometric capture (fingerprints, photo)
- SIM registration requires NIN (creating exclusion)
- NIN slip (paper) as fallback document
- NINAuth mobile app available

---

### 🇦🇪 UAE - UAE Pass (Production)

**Technology:** Cloud-based centralized identity  
**Services:** 12,000+ government and private services  
**Official Sources:**
- UAE Pass: https://www.uaepass.ae/
- Smart Dubai: https://www.smartdubai.ae/

**Technical Details:**
- One UAE Pass per person
- Linked to Emirates ID (physical ID card)
- Mobile app required for full functionality
- Digital vault for document storage
- Abu Dhabi, Dubai have separate systems

---

### 🇸🇦 Saudi Arabia - SDAIA (Specification)

**Technology:** Framework established, law pending 2026  
**Official Sources:**
- SDAIA: https://sdaia.gov.sa/
- Nafath: https://nafath.sa/

**Technical Details:**
- SDAIA (Saudi Data & AI Authority) framework launched
- Nafath for identity verification
- Digital ID law expected 2026
- Multiple identity providers under framework

---

### 🇶🇦 Qatar - Digital ID (Production)

**Technology:** Multiple systems for different sectors  
**Official Sources:**
- Government Portal: https://www.gov.qa/
- Ministry of Interior: https://www.moi.gov.qa/

**Technical Details:**
- Digital ID for healthcare, residency, employment
- Digital IDP (Identity Provider) available
- Physical documents still primary

---

### 🇴🇲 Oman - PKI-Based (Production)

**Technology:** PKI smart cards  
**Program:** Tawahul  
**Official Sources:**
- Oman Government: https://www.oman.om/
- Oman's Digital Transformation: https://www.oman.om/

**Technical Details:**
- PKI smart cards with digital certificates
- Tawahul program at 94% performance rating
- Government services integration

---

### 🇰🇪 Kenya - eCitizen (Production)

**Technology:** Cloud-based browser access  
**Official Sources:**
- eCitizen: https://www.ecitizen.go.ke/
- Huduma Centres: https://huduma.go.ke/

**Technical Details:**
- Browser-based (any device with browser)
- National ID required for SIM registration
- Huduma Centres provide one-stop government services
- SIM-NIN linkage required

---

### 🇧🇷 Brazil - RG Digital (Production)

**Technology:** Physical card with QR + mobile app  
**Since:** 2017  
**Official Sources:**
- Gov.br: https://www.gov.br/
- RG Digital: https://www.gov.br/pt-br/servicos/solicitar-segunda-via-do-rg

**Technical Details:**
- One RG (national ID) per citizen
- Digital version in gov.br app
- QR code on physical cards
- State-level implementation (varied)

---

### 🇦🇺 Australia - myGov ID (Production)

**Technology:** Cloud-based federated identity  
**Official Sources:**
- myGov ID: https://www.mygov.id.gov.au/
- Digital Transformation Agency: https://www.dta.gov.au/

**Technical Details:**
- Federal system, not state-issued
- Cloud-linked identity
- States have additional programs (NSW, Victoria)
- myGov for service access

---

### 🇲🇾 Malaysia - MyDigital ID (Production)

**Technology:** PKI-based with centralized registration  
**Target:** 15M users by end 2025  
**Official Sources:**
- Digital Government: https://www.digital.gov.my/
- MDEC: https://www.mdec.my/

**Technical Details:**
- If phone lost/damaged, must revoke at kiosk before re-registering
- Government kiosks for registration/revocation
- FIDO2/WebAuthn support

---

### 🇮🇱 Israel - Biometric ID (Production)

**Technology:** Biometric smart cards + app  
**Readiness Score:** 79/100  
**Official Sources:**
- Government Portal: https://www.gov.il/
- Ministry of Interior: https://www.gov.il/departments/ministry_of_interior

**Technical Details:**
- Biometric ID cards
- Gov.ID mobile app
- Physical card required

---

## Subnational Systems

### United States - Mobile Driver's Licenses (mDL)

**Technology:** Based on ISO/IEC 18013-5 (mDL standard)  
**TSA Accepted:** 11+ states  
**Official Sources:**
- AAMVA (Association of American Motor Vehicle Administrators): https://www.aamva.org/
- State DMVs individually

| State | mDL Launch | Platform | TSA | Official URL |
|-------|-------------|-----------|-----|--------------|
| Louisiana | 2018 | Expresslane (mobile-first) | ✓ | https://www.expresslane.org/ |
| Arizona | 2020 | Apple + Google Wallet | ✓ | https://www.azdot.gov/ |
| Maryland | 2021 | Apple + Google Wallet | ✓ | https://mva.maryland.gov/ |
| Colorado | 2022 | Apple + Google Wallet | ✓ | https://www.colorado.gov/dmv |
| Georgia | 2022 | Apple + Google Wallet | ✓ | https://dds.georgia.gov/ |
| Ohio | 2023 | Apple only | | https://www.bmv.ohio.gov/ |
| California | Dec 2023 | Apple Wallet | ✓ | https://www.dmv.ca.gov/ |
| Utah | 2023 | State app | ✓ | https://dld.utah.gov/ |
| Iowa | 2023 | State app | ✓ | https://iowadot.gov/ |
| Virginia | 2024 | Apple + Google Wallet | ✓ | https://www.dmv.virginia.gov/ |
| Nevada | 2024 | Apple + Google Wallet | ✓ | https://dmv.nv.gov/ |
| Vermont | 2024 | State app | ✓ | https://dmv.vermont.gov/ |
| New York | 2024 | State app | ✓ | https://dmv.ny.gov/ |
| New Jersey | 2025 (law) | TBD | | https://www.nj.gov/mvc |
| Texas | In dev | TBD | | https://www.txdps.gov/ |

---

### Canada - Provincial Digital IDs

**Technology:** Various (PKI, mobile apps, centralized)  

| Province | Program | Status | Official URL |
|----------|---------|--------|--------------|
| British Columbia | BC Wallet (Person Credential) | **LIVE** | https://www2.gov.bc.ca/gov/content/governments/government-id/bc-wallet |
| Alberta | Digital ID | Development | https://www.alberta.ca/ |
| Ontario | ServiceOntario | Production | https://www.ontario.ca/page/serviceontario |
| Quebec | Identité numérique Québec | Development | https://www.quebec.ca/ |
| Manitoba | Manitoba ID | Production | https://www.gov.mb.ca/ |
| Saskatchewan | eSask | Production | https://www.saskatchewan.ca/ |

**BC Details:**
- Person Credential now LIVE in BC Wallet
- BC Services Card also available
- One credential per person
- Mobile app-based

---

### Australia - State Programs

| State | Program | Status | Official URL |
|-------|---------|--------|--------------|
| NSW | Digital ID | Live | https://www.nsw.gov.au/ |
| Victoria | Digital Services | Live | https://www.vic.gov.au/ |

---

## No-Device Solutions

### Overview

Most systems assume smartphone/device ownership. Approaches for inclusion:

| Approach | Countries | How It Works |
|----------|-----------|--------------|
| **QR on Plastic** | Greece, Brazil | Static/dynamic QR codes on physical ID cards |
| **Biometric Kiosks** | India, Kenya | 100K+ Aadhaar centres, Huduma centres |
| **OTP Fallback** | India, others | SMS/email one-time passwords |
| **Community Access** | India (banking correspondents), Kenya (Huduma) | Shared devices in rural areas |
| **Paper Documents** | Nigeria (NIN slip), India (PVC Aadhaar) | Physical documents with verification |
| **Service Exclusion** | Nigeria | 73M blocked from mobile for lacking NIN |

---

## Key Takeaways for BC

1. **Technology Trends:** Moving toward wallet architecture (EUDI, US mDL) but significant variation remains

2. **Multi-Device Support:** Most systems are single-device; few support multiple devices

3. **Interoperability:** EUDI Wallet will set new standard for cross-border

4. **Inclusion:** Significant gap in no-device solutions globally; BC should prioritize this

5. **Standards:** ISO 18013-5 (mDL) gaining traction but not universal

---

## References

- European Commission: https://commission.europa.eu/
- UK Digital Identity: https://www.gov.uk/government/collections/uk-digital-identity-and-attributes-trust-framework
- UIDAI: https://uidai.gov.in/
- Singpass: https://www.singpass.gov.sg/
- e-Estonia: https://e-estonia.com/
- BankID: https://www.bankid.com/
- BSI Germany: https://www.bsi.bund.de/
- AAMVA: https://www.aamva.org/
- Gov.br: https://www.gov.br/
- myGov ID: https://www.mygov.id.gov.au/

---

*Last Updated: 2026-02-27*
