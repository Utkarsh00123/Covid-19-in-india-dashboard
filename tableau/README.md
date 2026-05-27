# Tableau Workbook

Place the packaged Tableau workbook file here:

```
tableau/Covid19_India_Dashboard.twbx
```

## Requirements

- **Tableau Desktop** 2020.1 or later, OR
- **[Tableau Public](https://public.tableau.com/app/discover)** (free) — download and open `.twbx` files

## How to Open

1. Download and install [Tableau Public](https://public.tableau.com/app/discover) (free) or Tableau Desktop
2. Double-click `Covid19_India_Dashboard.twbx`, OR
3. Open Tableau → **File → Open** → navigate to this file

## Sheets in the Workbook

| Sheet Name | Visualization |
|---|---|
| `Title` | Dashboard title slide |
| `1st vs Second dose administra...` | Bar chart — 1st vs 2nd dose by state |
| `Doses administrated by vaccine` | Bar chart — doses per vaccine brand |
| `Age Group Details` | Donut chart — % cases by age band |
| `Gender without missing values` | Donut chart — Male vs Female |
| `ICMR Testing Labs in each state` | Horizontal bar — lab count per state |
| `Statewise Testing Details` | Stacked horizontal bar — samples breakdown |
| `Map: total deaths by state` | Filled map — deaths choropleth |
| `Covid cases by State/UT` | Dual-axis line chart — Confirmed/Cured/Deaths |
| `Dashboard 1` | Final assembled dashboard |

## Data Connections

The workbook connects to the following files (place them in `data/` before opening):

- `covid_19_india.csv`
- `ICMRTestingLabs.csv`
- `StatewiseTestingDetails.csv`
- `AgeGroupDetails.csv`
- `IndividualDetails.csv`
- `covid_vaccine_statewise.csv`

See [`data/README.md`](../data/README.md) for download links.
