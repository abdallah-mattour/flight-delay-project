# Flight Delay Project

> A complete data-science pipeline that predicts flight delays across five countries using publicly available aviation data.

**Course:** COMP4381 — Data Science and Analytics  
**Semester:** Spring 2026  
**Instructor:** Dr. Ahmed Sabbah  
**Institution:** Birzeit University — Faculty of Engineering and Technology

---

## Team Members

| Name | Student ID |
|---|---|
| Abdullah Mattour | 1223061 |
| Sa'ed Alamleh    | 1220276 |
| Mohammad Hmaid   | 1230302 |

---

## Project Description

Flight delays are a costly, daily reality for airlines, airports, and millions of passengers around the world. This project builds a reproducible, end-to-end data-science pipeline that:

1. Collects raw aviation data from stable, public sources.
2. Cleans, filters, and merges it into a single analytical dataset that meets the course's minimum requirements (1,000+ rows, 15+ meaningful features, 5+ countries).
3. Explores the data through descriptive statistics and visualisations.
4. Trains a simple machine-learning model that predicts a delay-related target.
5. Discusses what the results mean, why they matter, and what limitations remain.

### Countries Covered

We cover **five European countries**, all reported through a single, consistent data source (EUROCONTROL), which keeps cleaning and merging straightforward:

- 🇬🇧 United Kingdom
- 🇩🇪 Germany
- 🇫🇷 France
- 🇳🇱 Netherlands
- 🇪🇸 Spain

### Prediction Target

The exact target variable is finalised in Phase 3, but our current plan is to predict either:

- **Average arrival delay (in minutes)** — a regression task, or
- **Delayed vs. on-time** (delay > 15 min) — a binary-classification task.

The choice between the two is documented in Notebook 03, after we have inspected the data.

---

## Data Sources

All datasets are public and downloaded from **stable URLs at notebook runtime** — there are no manual downloads.

| Source | URL | Used for |
|---|---|---|
| OurAirports — `airports.csv` | <https://davidmegginson.github.io/ourairports-data/airports.csv> | Airport metadata: type, latitude, longitude, elevation, region, municipality, scheduled-service flag |
| OurAirports — `countries.csv` | <https://davidmegginson.github.io/ourairports-data/countries.csv> | ISO country code lookup |
| OurAirports — `runways.csv` | <https://davidmegginson.github.io/ourairports-data/runways.csv> | Runway-level features (length, surface, count) |

The delay / punctuality dataset is finalised in Phase 3 and added here once selected.

---

## Repository Structure

```
flight-delay-project/
|-- README.md
|-- requirements.txt
|-- .gitignore
|-- data/
|   |-- raw/         # Untouched files downloaded from the source
|   `-- processed/   # Cleaned and merged datasets used for modelling
|-- notebooks/
|   `-- 00_welcome.ipynb
|-- report/          # PDF deliverables for each phase
`-- figures/         # Plots exported for the report
```
