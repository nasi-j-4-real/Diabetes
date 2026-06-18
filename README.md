### Student Project Report: Key Observations

#### Section 1: Pandas Missing Data Gaps
* **The Hidden Zero Bug**: Checking `.min()` exposes a major data-entry issue where impossible `0` entries are used as placeholders instead of blank cells.
* **Corrupted Metrics**: This flaw ruins **50% of Insulin** and **30% of SkinThickness** records, alongside critical entries in `Glucose`, `BMI`, and `BloodPressure`.
* **Extreme Skews**: The `.describe()` summary shows massive right-skewed ranges, especially for `Insulin` (max `846`).

#### Section 2: Profiling Trends & Correlations
* **Top Diagnosis Driver**: The **Correlations Heatmap** confirms **`Glucose`** holds the strongest positive link to a positive diabetes **`Outcome`**.
* **Body Metric Cluster**: A tight positive correlation ties **`BMI` vs. `SkinThickness`**, proving higher body mass directly tracks with thicker triceps skinfolds.
* **Age Patterns**: **`Age` vs. `Pregnancies`** displays a clear linear trend. Both features exhibit sharp, right-skewed curves, confirming our cohort consists mostly of younger patients.
