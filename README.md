# Tel Aviv Micromobility — Crash Analysis & Benchmarking (Phase 2)

**E-Scooter Safety Analytics · Phase 2 of 4**
Part of a longitudinal multi-phase research project on micro-mobility safety in Israel.
Presented at ISTRC Conference, Technion, January 2026.

---

## Live demo

▶ **[View interactive report](https://app.powerbi.com/view?r=eyJrIjoiNzVjNzBmNGItMDMxYi00MzFiLTk5NWEtNzFmODNlYzRkYjQzIiwidCI6IjE1YTgyNWJhLWE0ZjItNGE0Zi1hNzU5LWYyMzFlYjU4NzIwZCJ9)**
🎥 **[Demo video](MicroVehiclesDashboardVideo.mp4)**
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

| Page | Content |
|---|---|
| Overview | Crash volume trends, mode breakdown, YoY comparison |
| Severity analysis | Fatal/serious rates by mode, z-score significance testing |
| Benchmarking | Tel Aviv vs Israel national rates |
| Time patterns | Hour of day, day of week, seasonality |
| Demographics | Age groups, gender, population type |
| Road conditions | Road type, lighting, speed limits, intersection control |
| Mode deep-dive | Per-mode statistics with significance tests |
| AI visuals | Key Influencers, Decomposition Tree |

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
├── README.md                          ← this file
├── pbix/
│   └── micro_accidents_TA_jul17.pbix  ← Power BI Desktop report
├── media/
│   └── MicroVehiclesDashboardVideo.mp4  ← demo walkthrough video
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
