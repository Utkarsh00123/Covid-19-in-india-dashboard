# Data Dictionary

Field-by-field description of every CSV file used in the dashboard.

---

## `covid_19_india.csv`

| Column | Type | Description |
|---|---|---|
| `Sno` | Integer | Serial number |
| `Date` | Date (DD/MM/YYYY) | Date of record |
| `Time` | String | Time of update |
| `State/UnionTerritory` | String | State or UT name |
| `ConfirmedIndianNational` | Integer | Confirmed Indian nationals |
| `ConfirmedForeignNational` | Integer | Confirmed foreign nationals |
| `Cured` | Integer | Cumulative recovered cases |
| `Deaths` | Integer | Cumulative deaths |
| `Confirmed` | Integer | Total cumulative confirmed cases |

---

## `ICMRTestingLabs.csv`

| Column | Type | Description |
|---|---|---|
| `State` | String | State or UT name |
| `Lab` | Integer | Number of ICMR-approved testing labs |

> **Note:** Maharashtra (39) has the highest lab count, followed by Tamil Nadu (26) and Telangana (19).

---

## `StatewiseTestingDetails.csv`

| Column | Type | Description |
|---|---|---|
| `Date` | Date | Date of record |
| `State` | String | State or UT name |
| `TotalSamples` | Integer | Cumulative total samples tested |
| `Negative` | Integer | Cumulative negative results |
| `Positive` | Integer | Cumulative positive results |

---

## `AgeGroupDetails.csv`

| Column | Type | Description |
|---|---|---|
| `Sno` | Integer | Serial number |
| `Age Group` | String | Age band (e.g., `0-9`, `10-19`, ..., `80+`, `Missing`) |
| `TotalCases` | Integer | Count of confirmed cases in this age group |
| `Percentage` | Float | Percentage of total confirmed cases |

> **Key stats from dashboard:** 20-29 (24.86%), 30-39 (16.18%), 40-49 (16.18%), Missing (1.30%)

---

## `IndividualDetails.csv`

| Column | Type | Description |
|---|---|---|
| `id` | Integer | Row identifier |
| `age` | Integer / Null | Age of individual (may be missing) |
| `gender` | String | `M` (Male) or `F` (Female) |
| `detected_city` | String | City where case was detected |
| `detected_district` | String | District |
| `detected_state` | String | State |
| `current_status` | String | Current case status |
| `notes` | String | Additional notes |
| `contracted_from_which_patient_number` | String | Linked patient ID |
| `nationality` | String | Nationality |
| `type_of_transmission` | String | Imported / Local / Unknown |
| `status_change_date` | Date | Date of last status change |
| `source_1–3` | String | News/report sources |

> **Key stats from dashboard (gender without missing):** Male 66.76%, Female 33.24%

---

## `covid_vaccine_statewise.csv`

| Column | Type | Description |
|---|---|---|
| `Updated On` | Date | Date of data update |
| `State` | String | State or UT name |
| `Total Doses Administered` | Integer | Cumulative total doses given |
| `Sessions` | Integer | Vaccination sessions held |
| `Sites` | Integer | Vaccination sites |
| `First Dose Administered` | Integer | Cumulative 1st dose count |
| `Second Dose Administered` | Integer | Cumulative 2nd dose count |
| `Male (Doses Administered)` | Integer | Doses given to males |
| `Female (Doses Administered)` | Integer | Doses given to females |
| `Transgender (Doses Administered)` | Integer | Doses given to transgender |
| `CoVaxin (Doses Administered)` | Integer | Covaxin doses |
| `Covishield (Doses Administered)` | Integer | Covishield doses |
| `Sputnik V (Doses Administered)` | Integer | Sputnik V doses |
| `18-44 Years (Doses Administered)` | Integer | Doses in 18-44 age group |
| `45-60 Years (Doses Administered)` | Integer | Doses in 45-60 age group |
| `60+ Years (Doses Administered)` | Integer | Doses in 60+ age group |
| `Total Individuals Registered` | Integer | Total registered for vaccination |
| `Total Individuals Vaccinated` | Integer | Total individuals vaccinated |
