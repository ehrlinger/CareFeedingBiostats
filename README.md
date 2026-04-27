# Care and Feeding of Your Biostats Team

[![Render and Deploy](https://github.com/ehrlinger/CareFeedingBiostats/actions/workflows/deploy.yml/badge.svg)](https://github.com/ehrlinger/CareFeedingBiostats/actions/workflows/deploy.yml)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Made with Quarto](https://img.shields.io/badge/Made%20with-Quarto-blue)](https://quarto.org)
[![R/Medicine 2026](https://img.shields.io/badge/R%2FMedicine-2026-276DC3)](https://rconsortium.github.io/RMedicine/)

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

## Speaker Bio

John Ehrlinger is Assistant Staff and Lead Data Scientist in the Department of Cardiothoracic Surgery at the Heart, Vascular & Thoracic Institute (HVTI), Cleveland Clinic. He holds a joint appointment as Clinical Assistant Professor at the Cleveland Clinic Lerner College of Medicine. He leads a mixed team of data engineers and biostatisticians supporting cardiovascular outcomes research across large multi-institutional registries.

John earned his PhD in Statistics from Case Western Reserve University in 2011, where he worked with Hemant Ishwaran on ensemble methods for high-dimensional survival data. His methodological interests include survival analysis, random forests, and reproducible research infrastructure for clinical teams. He is an active R package author — his packages include `ggRandomForests`, `boostmtree`, and `TemporalHazard` — and has led the development of internal tooling (`hvtiPlotR`, `hvtiRutilities`) to standardize analysis workflows across a 19-person hybrid SAS/R team.

---

## Slides

View the live deck at [ehrlinger.github.io/CareFeedingBiostats](https://ehrlinger.github.io/CareFeedingBiostats).

Built with [Quarto](https://quarto.org/) revealjs. To render locally:

```r
quarto::quarto_render("index.qmd")
```

Or from the terminal:

```bash
quarto render index.qmd
```

---

## Packages Referenced

| Package | Description |
|---|---|
| [`ggRandomForests`](https://github.com/ehrlinger/ggRandomForests) | ggplot2 visualizations for randomForestSRC |
| [`hvtiPlotR`](https://github.com/ehrlinger/hvtiPlotR) | CORR-standard ggplot2 themes and plot types |
| [`hvtiRutilities`](https://github.com/ehrlinger/hvtiRutilities) | R job governance checks |
| [`hazard`](https://github.com/ehrlinger/hazard) | SAS multi-phase hazard analysis |
| [`TemporalHazard`](https://github.com/ehrlinger/temporal_hazard) | Native R port of the SAS/C hazard code |
