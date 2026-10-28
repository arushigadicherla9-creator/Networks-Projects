# Title 

The repository contains code accompanying the following paper: Cody Chhea, Arushi Gadicherla, and Lisa Hires, *Measles Transmission Risk Through the U.S. Flight Network and State-Level Vaccination Coverage* (2026).

This project builds a directed, weighted network of 2025 U.S. domestic air travel and combines it with state-level MMR vaccination coverage and confirmed 2025 measles cases. Airports are first connected by edges weighted by annual passenger volume, then aggregated into a state-level network. We use network measures (degree, weighted degree, betweenness centrality, and effective distance) to examine whether states with high flight connectivity and low vaccination coverage face greater measles transmission risk.

If you use this repository in any fashion in your own work, please cite our work according to the `CITATION.cff`.

# Contents

- [Contents](#contents)
- [Getting Started](#getting-started)
  - [Repository layout](#repository-layout)
  - [Data sources](#data-sources)
  - [Installation](#installation)
- [Other Information](#other-information)
  - [Authors](#authors)
  - [License](#license)

# Getting started

## Repository layout

| Path | Role |
|---|---|
| `data/` | Raw and cleaned datasets (flight data, measles cases, MMR vaccination coverage) |
| `code/` | Python scripts for data cleaning, network construction, and network analysis |
| `<FLIGHT DATA FILE>` | 2025 BTS domestic flight data with passengers, origin, and destination |
| `<MEASLES DATA FILE>` | 2025 confirmed measles cases by county, from the JHU Measles Tracking Team |
| `<MMR DATA FILE>` | 2024–2025 county-level MMR vaccination coverage from Dong et al. (2025) |
| `<CLEANING SCRIPT>` | Removes zero-passenger flights, unused columns, and null values; filters to 2025 |
| `<NETWORK SCRIPT>` | Builds the airport-level network and aggregates it to the state level |
| `<ANALYSIS SCRIPT>` | Calculates degree, weighted degree, betweenness centrality, and effective distance |
| `requirements.txt` | Python packages needed to run the code |

## Data sources

| Dataset | Source | Link |
|---|---|---|
| 2025 domestic flights (BTS2025) | U.S. Bureau of Transportation Statistics | https://www.transtats.bts.gov/ |
| 2025 confirmed measles cases | JHU Measles Tracking Team Data Repository at Johns Hopkins University | https://github.com/CSSEGISandData/measles_data |
| 2024–2025 MMR vaccination coverage | Dong et al., "Trends in County-Level MMR Vaccination Coverage in Children in the United States," *JAMA* (2025) | https://github.com/CSSEGISandData/MMR_data |

## Installation

```bash
pip install -r requirements.txt
```

# Other information

## Authors

- Cody Chhea (psh7rp@virginia.edu)
- Arushi Gadicherla (yte6zv@virginia.edu)
- Lisa Hires (uar2aw@virginia.edu)

Department of Biology, University of Virginia

## License

This project is licensed under the [BSD-3 License](LICENSE) - see the [LICENSE](LICENSE) file for details.
