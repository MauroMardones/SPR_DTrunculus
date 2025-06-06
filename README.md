
# SPR Assessment of wedge clam *Donax trunculus* in the Gulf of Cádiz using LBSPR

## Overview

This repository contains the code, data, and outputs related to the estimation of the **Spawning Potential Ratio (SPR)** of the coquina clam (*Donax trunculus*) in the Gulf of Cádiz, using the **Length-Based Spawning Potential Ratio (LBSPR)** model as described by Hordyk et al. (2015).

The analysis focuses on the coastal area adjacent to **Doñana National Park**, where a long-term artisanal fishery monitoring program has been conducted for over a decade under the **FEMP 04** initiative.

## Objectives

* Estimate the current SPR of *Donax trunculus* using length frequency data.
* Evaluate exploitation status relative to biological reference points.
* Support sustainable management of this artisanal fishery in a sensitive ecological area.

## Data Source

* **FEMP 04 Monitoring Program**
  Length frequency and environmental data have been collected regularly over the past **10 years** from the artisanal coquina fishery in the Doñana region.

## Methodology

The **LBSPR** model (Hordyk et al., 2015) is applied to the length composition data to estimate:

* Spawning Potential Ratio (SPR)
* Selectivity parameters (SL50 and SL95)
* Estimates of fishing mortality relative to life history parameters

### References

* Hordyk, A.R., Ono, K., Valencia, S.R., Loneragan, N.R., & Prince, J.D. (2015). A novel length-based empirical estimation method of spawning potential ratio (SPR), and tests of its performance, for small-scale, data-poor fisheries. *ICES Journal of Marine Science*, **72**(1), 217–231. [https://doi.org/10.1093/icesjms/fsu004](https://doi.org/10.1093/icesjms/fsu004)

## Repository Structure

```
.
├── data/           # Raw and processed length-frequency data (from FEMP 04)
│   └── femp04_lengths_2014_2024.csv
│
├── modelo/         # R scripts and LBSPR model implementation
│   └── run_lbspr_model.R
│
├── outputs/        # SPR estimates, diagnostic plots, model results
│   ├── spr_results_summary.csv
│   └── plots/
│       └── spr_trends.png
│
├── reporte/        # RMarkdown report for documentation and visualization
│   └── SPR_Doñana_Report.Rmd
│
└── README.md       # This file
```

## Requirements

This project is written in **R**, and requires the following packages:

* `LBSPR`
* `tidyverse`
* `here`
* `rmarkdown`

You can install the LBSPR package from CRAN:

```r
install.packages("LBSPR")
```

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/MauroMardones/SPR_DTrunculus.git
```

2. Open the R project or the main script `run_lbspr_model.R` located in `/modelo`.

3. Execute the RMarkdown file `SPR_Doñana_Report.Rmd` to generate the full report.

## Contact

For any questions or contributions, please contact:
**Mauricio Mardones**
*Fisheries Researcher – IEO, Cádiz, Spain*
Email: [mauricio.mardones@ieo.csic.es](mauricio.mardones@ieo.csic.es)

