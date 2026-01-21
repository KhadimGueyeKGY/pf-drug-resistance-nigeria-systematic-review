# Plasmodium falciparum molecular drug resistance in Nigeria (2000–2024)
**Systematic review + curated supplementary tables + reproducible figures & analyses**

This repository contains the curated data tables (S1–S6), the analysis notebook used to generate the manuscript figures, and draft manuscript materials for a systematic review of *Plasmodium falciparum* molecular antimalarial drug resistance markers in Nigeria.

---

## Repository contents

- `malaria_drug_resistance_figures_analysis.ipynb`  
  Main notebook to load the curated tables, generate figures (main + supplementary), and run example statistical analyses.

- `data/`  
  Curated supplementary tables used for analysis (Excel files S1–S6).

- `plot/` 
  Output folders used for exported figures and intermediate plots (structure may vary depending on your workflow).

---

## What the notebook does

### Data
- Loads curated supplementary tables (S1–S6).
- Harmonizes year fields (e.g., **corrected year**) and converts prevalence fields to proportions.
- Uses Nigerian samples only when the table includes “Nigeria only” sample size fields.

### Figures generated
- **Figure 1** – PRISMA flow diagram (publication-ready style)
- **Figure 2A–D** – Study metrics (markers studied, population types, country of sample collection, studies per year)
- **Figure 3** – pfcrt K76T prevalence over time
- **Figure 4A–B** – pfmdr1 mutation prevalence + trends
- **Figure 5A–D** – pfdhfr & pfdhps prevalence and combined haplotypes
- **Figure S1** – additional pfdhps mutations over time (multi-panel)
- **Figure 6** – pfkelch13 mutations (summary + prevalence patterns)


> Note: The repository is designed to be **reproducible**. Figures are generated directly from the curated tables.

---

## Requirements

Recommended environment (Python ≥ 3.9):

- pandas
- numpy
- matplotlib
- scipy (optional, for some stats)
- statsmodels (recommended for regressions)
- openpyxl (Excel I/O)

Install with:

```bash
pip install pandas numpy matplotlib scipy statsmodels openpyxl
