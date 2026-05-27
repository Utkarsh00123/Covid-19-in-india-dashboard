# 📁 Data Sources

> **No CSV files are committed to this repository** to keep the repo lightweight.  
> Download the datasets directly from the sources below.

---

## 🔗 Primary Dataset — Kaggle

**[COVID-19 in India — sudalairajkumar](https://www.kaggle.com/datasets/sudalairajkumar/covid19-in-india)**

This single dataset contains most of the files used in this project:

| File | Description |
|---|---|
| `covid_19_india.csv` | Date-wise confirmed, cured, deaths per state/UT |
| `StatewiseTestingDetails.csv` | Cumulative total, positive & negative samples per state |
| `ICMRTestingLabs.csv` | ICMR-approved testing lab count per state |
| `AgeGroupDetails.csv` | COVID cases broken down by age band |
| `IndividualDetails.csv` | Individual-level records including gender |
| `covid_vaccine_statewise.csv` | 1st and 2nd dose vaccination counts per state |

---

## 🔗 Secondary Dataset (Vaccination Details)

**[COVID-19 Vaccine Statewise — anmolkumar](https://www.kaggle.com/datasets/anmolkumar/covid19-vaccine-statewise)**

Used for the vaccination sheets (1st vs 2nd dose, doses administered by vaccine type).

---

## 🗺️ India States Shapefile (for Map Visualization)

Required to build the **"Map: Total Deaths by State"** choropleth in Tableau.

**Option 1 — Tableau Built-in:**  
Use Tableau's native geographic role (`State/Province`) — works without a shapefile if state names match correctly.

**Option 2 — Custom Shapefile:**  
Download from [GADM India Boundaries](https://gadm.org/download_country.html) → select **India** → Level 1 → Shapefile format.

---

## 📥 How to Download from Kaggle

1. Create a free account at [kaggle.com](https://www.kaggle.com)
2. Go to the dataset link above
3. Click **Download** (top-right) — a ZIP archive will be saved
4. Extract into this `data/` folder

After extracting, your `data/` folder should look like:

```
data/
├── README.md                          ← (this file)
├── covid_19_india.csv
├── StatewiseTestingDetails.csv
├── ICMRTestingLabs.csv
├── AgeGroupDetails.csv
├── IndividualDetails.csv
├── covid_vaccine_statewise.csv
└── india_states_shapefile/            ← (optional, for custom map)
    ├── gadm41_IND_1.shp
    └── ...
```
