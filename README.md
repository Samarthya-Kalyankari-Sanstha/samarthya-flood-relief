# Samarthya Madat Programme — Marathwada Flood Relief 2025

**Impact documentation dashboard** for the emergency flood relief response by **Samarthya Kalyankari Sanstha**, a women-led grassroots organisation working with De-notified and Nomadic Tribe (DNT) communities in Osmanabad (Dharashiv), Maharashtra.

**Live dashboard:** https://samarthya-kalyankari-sanstha.github.io/samarthya-flood-relief/

---

## About the Madat Programme

Following the September 2025 floods in Osmanabad district, Samarthya distributed **3,000 dry ration kits** across **55 habitations** in Omerga and Lohara blocks between September 2025 and March 2026. Every distribution was GPS-tagged and photo-verified at the point of delivery.

Key figures documented on this dashboard:

- 3,000 beneficiary households across 55 habitations, individually recorded
- 68.3% female-headed households, above the IASC 50% standard
- 68.5% of households carried two or more simultaneous vulnerabilities
- 15-member field team, 80% women, all from DNT communities
- 99.1% of recipients received no other government or NGO assistance
- Post-Distribution Monitoring (April 2026): 111 household interviews, 12 FGDs, assessed against the 9 CHS commitments

The documentation is honest by design: findings that reflect areas for improvement, such as 85 of 111 PDM respondents describing the distribution as "somewhat late", are reported alongside the achievements.

## Dashboard contents

The dashboard has 8 sections:

1. **Overview** — headline figures, gender disaggregation, monthly distribution, flood context
2. **Reach & vulnerability** — 10-criteria vulnerability profiling of all 3,000 households
3. **Geographic map** — interactive Leaflet map of all 55 habitations; each dot opens a per-beneficiary photo pager with name and vulnerability profile
4. **Samarthya team** — the 15 field members and their records
5. **Accountability** — GPS, photo, and signature verification standards; the 13-step accountability workflow
6. **PDM report** — Post-Distribution Monitoring findings, community voices in Marathi and English
7. **CHS compliance** — assessment against the 9 Core Humanitarian Standard commitments
8. **Context & gallery** — flood background and field photographs

## Repository structure

```
index.html        Main dashboard (single page, ~105 KB)
map_data.json     Beneficiary map data — 3,000 records grouped by habitation
assets/           Dashboard images: logos, field photos, PDM photos, infographics
thumbs/           Beneficiary photo thumbnails (~320px), named by file ID
README.md         This file
```

The dashboard is a static site with no build step. `index.html` loads `map_data.json` on demand when the Geographic Map tab is opened, and images load progressively from `assets/` and `thumbs/`. Charts are rendered with Chart.js and the map with Leaflet.js (both via CDN).

### Beneficiary photos

Of the 3,000 beneficiary records, 2,965 have a verified photograph displayed in the map popups. For the remaining 35, no usable photograph exists in the source records (in most cases only a signature or thumb impression was captured); these are shown as "missing" rather than substituted, in line with the honest-reporting approach.

## Data sources

- **KoboToolbox** — 59 individual project forms; per-beneficiary records with GPS coordinates, timestamps, unique submission UUIDs, photo and acknowledgment evidence
- **Master dataset** — 40-column consolidated record of all 3,000 distributions
- **PDM survey** — 111 households, 7 enumerators, 2–18 April 2026

## Supported by

Primary funder: **Azim Premji Foundation (APF)**. Additional support from APPI, Mama Cash, WFA, and individual crowdfunding contributors.

## Contact

Samarthya Kalyankari Sanstha, Osmanabad (Dharashiv), Maharashtra
Helpdesk: 8888026292
