# Output

Processed data files made by the code in `code/`. Use these for all network analysis.

| File | Description |
|---|---|
| `airport_edges_2025.csv` | Network edges. Each row is a directed route (`origin`, `dest`) with total 2025 passengers. Only routes with at least 1,000 passengers are kept. |
| `nodes.csv` | One row per airport: name, state, latitude/longitude, and total passengers flying out and in. |
| `airport_attributes_2025.csv` | Airport table plus service-area summary: number of counties, 2025 measles cases, first case date, mean MMR coverage (`mmr_mean`), and percent of counties below 95% coverage. |
| `county_measles_mmr_2025.csv` | One row per U.S. county: location, 2025 measles cases, first case date, and 2024–25 kindergarten MMR coverage. |
| `county_nearest_airport.csv` | County table plus each county's nearest airport and distance to it (km). |
