# Care and Feeding of Your Biostats Team

**Scaling Best Practices in a Large Hybrid SAS/R Team**

A 20-minute recorded talk for [R/Medicine 2026](https://rconsortium.github.io/RMedicine/).

**Speaker:** John Ehrlinger, PhD
Assistant Staff, Lead Data Scientist
Heart, Vascular & Thoracic Institute
Cleveland Clinic

---

## Abstract

Running a large biostatistics team means managing analysts across two platforms — SAS and R — with varying levels of experience, informal conventions, and no shared enforcement layer. This talk covers the practical infrastructure we've built at Cleveland Clinic's Cardiovascular Outcome Registries and Research (CORR) to make analyses reproducible, transferable, and maintainable across a 19-person hybrid team.

Organized around three production steps — data ingestion, model building, and results and figures — the talk covers what we've adopted, what's in development, and what remains aspirational.

---

## Slides

Built with [Quarto](https://quarto.org/) revealjs. To render:

```r
quarto::quarto_render("CareFeeding.qmd")
```

Or from the terminal:

```bash
quarto render CareFeeding.qmd
```

---

## Packages Referenced

| Package | Description |
|---|---|
| [`ggRandomForests`](https://github.com/ehrlinger/ggRandomForests) | ggplot2 visualizations for randomForestSRC |
| [`hvtiPlotR`](https://github.com/ehrlinger/hvtiPlotR) | CORR-standard ggplot2 themes and plot types |
| [`hvtiPropensityScore`](https://github.com/ehrlinger/hvtiPropensityScore) | Standard propensity score matching workflow |
| [`hvtiRutilities`](https://github.com/ehrlinger/hvtiRutilities) | R job governance checks |
| [`hazard`](https://github.com/ehrlinger/hazard) | SAS multi-phase hazard analysis |
| [`temporal_hazard`](https://github.com/ehrlinger/temporal_hazard) | Native R port of the SAS/C hazard code |
| [`mixhazard`](https://github.com/ehrlinger/mixhazard) | Generalized hazard extension (not limited to 3 phases) |
