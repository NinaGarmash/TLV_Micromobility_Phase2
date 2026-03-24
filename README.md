# Tel Aviv Micromobility — Crash Analysis & Benchmarking (Phase 2)

**E-Scooter Safety Analytics · Phase 2 of 4**
Part of a longitudinal multi-phase research project on micro-mobility safety in Israel.
Presented at ISTRC Conference, Technion, January 2026.

---

## Live demo

▶ **[View interactive report](https://app.powerbi.com/view?r=eyJrIjoiNzVjNzBmNGItMDMxYi00MzFiLTk5NWEtNzFmODNlYzRkYjQzIiwidCI6IjE1YTgyNWJhLWE0ZjItNGE0Zi1hNzU5LWYyMzFlYjU4NzIwZCJ9)**
🎥 **[Demo video](media/MicroVehiclesDashboardVideo.mp4)**
🏆 **[Maven Analytics showcase](https://mavenshowcase.com/project/37454)**

---

## What this report covers

A deep comparative analysis of all micromobility crash data in Tel Aviv (2013–Jul 2024), benchmarking e-scooters against e-bikes and bicycles across crash volume, injury severity, demographics, time patterns, and road conditions. This phase established the analytical framework — treating **crash volume and severity as two independent dimensions** — that became central to the entire research project.

| Attribute | Value |
|---|---|
| **Geography** | Tel Aviv–Yafo |
| **Years** | 2013–Jul 2024 |
| **Total accidents** | 8,671 |
| **Total people involved** | 17,395 |
| **Modes compared** | E-Scooter · E-Bike · Bicycle (+ other micro) |
| **Tool** | Power BI Desktop |
| **Data source** | CBS Israel crash microdata |

---

## Key findings

- **E-scooters dominate crash volume** among micro-mobility modes, especially post-2021
- **Volume ≠ Severity**: the modes with the most crashes are not the same as the modes with the highest injury rates — a central finding of the analysis
- Of 8,671 accidents: **640 serious** (7.4%), **40 fatal** (0.5%), **7,991 light** (92.1%)
- **E-bikes show higher severity rates** than e-scooters despite lower crash volume — this divergence widened post-2022
- **AI-powered features** (Key Influencers, Q&A visual, Decomposition Tree) enable non-expert municipal staff to explore data independently

### Involved persons by mode (Tel Aviv, 2013–Jul 2024)

| Mode | People involved |
|---|---|
| E-Bike (אופניים חשמליים) | 3,554 |
| Bicycle (אופניים) | 3,237 |
| E-Scooter (קורקינט חשמלי) | 2,224 |
| Other micromobility | 111 |

---

## Report pages

The report contains **20 numbered pages** plus a Contents navigation page, grouped into 5 sections. An additional 14 supporting pages (statistical test details, drill-through targets, tooltips) are hidden from the main navigation.

### Section A — Introduction & Overview

| Page | Title | Content |
|------|-------|---------|
| — | Contents | Navigation page |
| 1 | Israel–TA Intro | Tel Aviv has 16% micromobility crash share — nearly 3× the national average (5.6%); e-scooters account for 38% of Israel's e-scooter crashes |
| 2 | TA Micro Mode, Location | Crash map with dense city-centre clustering; top streets (Begin Rd, Ibn Gvirol, Dizengoff); mode breakdown (e-bikes 39.5%, bicycles 36.4%, e-scooters 24.7%) |
| 3 | Vehicles & Involved | Crash complexity: 83% of crashes involve 2 people, 76% involve 2 vehicles; micromobility vehicles are 56.2% of all involved vehicles |

### Section B — Trends & Time Patterns

| Page | Title | Content |
|------|-------|---------|
| 4 | Micro Trends | Year-over-year mode dynamics; e-scooter crashes rose sharply since 2017, reaching 45% of micromobility crashes in 2023–2024; bikes declining, e-bikes stable |
| 5 | Accidents: Time Patterns | Crashes peak in summer (May–Sep) and daytime (08–17h); e-scooter share rises at night (00–03h); weekday vs. weekend differences by mode |
| 6 | Time Patterns Tested | Statistical significance of timing differences by mode; e-scooters show summer & night spikes; bikes show weekend bias; modes are not interchangeable for safety planning |

### Section C — Severity

| Page | Title | Content |
|------|-------|---------|
| 7 | Injury & Accident Severity over Years | Severity trends 2013–2024; fatalities by mode (e-bikes 18, bikes 14, e-scooters 9); accident severity rising ~8% annually; e-scooter riders show highest year-over-year severity |
| 8 | Accident Severity: Time Patterns | E-scooter severity rate = 10.3% (highest of all modes); severity peaks in April & November, at 03:00 and 20:00, and midweek/Saturdays |
| 9 | DOW × Hour Heatmaps | Hour-of-day × day-of-week heatmap for all crashes vs. severe crashes; severe accidents cluster on Friday early morning (04–06h); night severity rate >30% |
| 10 | All–Micro Users Severity | Severity by age (highest for <15 and >65), gender (males more severely injured), and population type (foreigners at highest risk); most riders aged 25–29 |
| 11 | Severity: Socio-Demographic Factors Tested | Statistical tests by mode across all demographic groups; e-scooters most dangerous in every comparison; bicycles safest |
| 12 | Severity – Environmental Factors | Impact of lighting (night raises severity), road type, intersection control (absent control = more severe), and road surface defects |
| 13 | Severity – Other Factors | E-scooter focus: crash type (overturning/sliding most severe), seating position (rear-seated/standing = 100% severity in small samples), safety gear (no helmet = 70% severity vs. 55% with protection) |
| 14 | Severity by Mode Test | Cross-mode comparison across all environmental and behavioural conditions; e-scooters worst at intersections and without safety gear; bicycles safest at uncontrolled roads |

### Section D — Drivers & Victims

| Page | Title | Content |
|------|-------|---------|
| 15 | Driver, Passenger, Pedestrian | Role distribution: drivers 3,886, victims 310 (7.4%); victim severity 15% vs. driver severity 5%; highest victim share among women and seniors |
| 16 | Drivers & Non-Drivers by Mode | Victim share by mode; e-scooters show higher non-rider victim share especially among elderly; women more likely to be victims when switching from bike to scooter/e-bike; foreigners and Arabs have higher victim share across all modes |
| 17 | Involved Decomposition | AI Decomposition Tree exploring factors behind severe outcomes among all involved persons |
| 18 | Accidents Decomposition | AI Decomposition Tree exploring factors behind accident severity at the crash level |

### Section E — Conclusions

| Page | Title | Content |
|------|-------|---------|
| 19 | Conclusions | Key takeaways: TA has triple the national micromobility crash rate; e-scooters lead in both volume and severity; nighttime and summer are high-risk periods; victim risk shaped by age, gender, protection, and setting |
| 20 | Recommendations | Policy recommendations: e-scooters require urgent dedicated regulation; different micromobility modes must not be treated the same in safety planning |

---

## Data model highlights

The model contains **21 tables** and **~100 measures**, including:
- Separate fact tables per mode (`involved_TA_micro`, `vehicles_TA_micro`, `markers_TA_micro`)
- `_Measures` table centralising all calculations
- Statistical significance measures: z-scores, p-values per mode comparison
- `Accident_Flat` and `Accident Tier` tables for severity tiering
- Seasonality dimension tables (month, day-of-week, hour)

---

## Files in this repo

```
TLV_Micromobility_Phase2/
├── README.md                            ← this file
├── pbix/
│   └── micro_accidents_TA_jul17.pbix    ← Power BI Desktop report (Git LFS)
├── media/
│   └── MicroVehiclesDashboardVideo.mp4  ← demo walkthrough video (Git LFS)
└── data/
    └── (CBS source data not included — see Data Sources below)
```

---

## Data sources

**CBS Israel** — Central Bureau of Statistics road accident microdata.
Available at: [data.gov.il](https://data.gov.il/dataset/road_accidents_with_casualties_israel)
Scope: Tel Aviv–Yafo accidents involving at least one micromobility vehicle (e-scooter, e-bike, bicycle, electric scooter).
Data cut: January 2013 through July 2024.

---

## How this fits into the project

```
Phase 1  →  Phase 2  →  Phase 3a/3b  →  Phase 4
National     Tel Aviv     Tel Aviv         Tel Aviv
all modes    micromobility  e-scooters     full integration
             (this repo)    CBS 2013–2025  + surveys + enforcement
```

← **Phase 1**: [road_accidents_project](../road_accidents_project)
→ **Phase 3**: [Road_Accidents_in_Israel-2013-2024](../Road_Accidents_in_Israel-2013-2024)
→ **Phase 4**: [Escooter_TLV_Safety_Phase4](../Escooter_TLV_Safety_Phase4)

---

## Author

**Nina Garmash, PhD**
ANYWAY Project (DATA FOR CHANGE) · HIT (Holon Institute of Technology)
[LinkedIn](https://www.linkedin.com/in/nina-garmash) · [Portfolio](https://ninagarmash.wixsite.com/data-showcase)
