# NASA2025_project

# Exoplanet Detection and Classification

Welcome to the Exoplanet Detection and Classification project! This project leverages machine learning to automate the detection and classification of exoplanets using data from NASA's space telescopes. Our goal is to streamline the analysis of astronomical data, reducing manual workload and improving consistency.

## Project Overview

This project processes observational data from three NASA space telescopes—TESS, Kepler, and K2—to identify and classify exoplanets using a multi-stage machine learning model. The data, sourced from open NASA archives, is preprocessed to ensure consistency across different telescope datasets. Our web application allows scientists, enthusiasts, and space lovers to explore exoplanet data and predict whether an object is an exoplanet.

Explore the results and interact with the model on our [website](#) (link to be added).

## Data and Sources

Our data is sourced from the following open NASA resources:
- [NASA Exoplanet Archive — Cumulative Table](https://exoplanetarchive.ipac.caltech.edu/)
- [NASA Exoplanet Archive — TESS Objects of Interest](https://exoplanetarchive.ipac.caltech.edu/)
- [NASA Exoplanet Archive — K2 Candidates and Confirmed](https://exoplanetarchive.ipac.caltech.edu/)

### Data Challenges
All three telescopes (TESS, Kepler, K2) use the transit method for observations, but their data formats are inconsistent. To address this, we performed extensive data analysis and preprocessing to normalize the datasets into a comparable form. Key results from this analysis are available on our website.

## Problem Statement

Manually processing satellite observations for exoplanet detection is time-consuming and subject to inconsistent interpretations among astronomers. Our solution is a machine learning model that automates the detection and classification of exoplanets, improving efficiency and consistency.

## Web Application

Our web application is designed for scientists, space enthusiasts, and anyone curious about the universe. It features:
- A four-level architecture powered by a multi-stage machine learning classification model.
- A user-friendly interface to input data and receive the probability that an object is an exoplanet.
- Visualizations of confirmed exoplanetary systems and their host stars.

## Model Performance Metrics

The machine learning model was trained and evaluated on data from TESS, Kepler, and K2 satellites. Below are the performance metrics for each satellite and stage of the model.

### K2 Satellite
- Stage 1
  - AUC: 0.9488
  - F1: 0.9585
  - Accuracy: 0.93
  - Metrics Table:

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.52      | 0.76   | 0.62     | 63      |
| 1     | 0.98      | 0.94   | 0.96     | 738     |
| Macro Avg | 0.75 | 0.85 | 0.79 | 801 |
| Weighted Avg | 0.94 | 0.93 | 0.93 | 801 |

- Stage 2 (Shrunk to first 213 iterations)
  - AUC: 0.9630
  - F1: 0.9397
  - Accuracy: 0.92
  - Metrics Table:

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.93      | 0.86   | 0.89     | 275     |
| 1     | 0.92      | 0.96   | 0.94     | 463     |
| Macro Avg | 0.92 | 0.91 | 0.92 | 738 |
| Weighted Avg | 0.92 | 0.92 | 0.92 | 738 |

### Kepler Satellite
- Stage 1 (Shrunk to first 374 iterations)
  - AUC: 0.9362
  - F1: 0.8510
  - Accuracy: 0.85
  - Metrics Table:

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.86      | 0.85   | 0.85     | 968     |
| 1     | 0.85      | 0.85   | 0.85     | 945     |
| Macro Avg | 0.85 | 0.85 | 0.85 | 1913 |
| Weighted Avg | 0.85 | 0.85 | 0.85 | 1913 |

- Stage 2 (Shrunk to first 436 iterations)
  - AUC: 0.9485
  - F1: 0.9111
  - Accuracy: 0.89
  - Metrics Table:

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.85      | 0.85   | 0.85     | 341     |
| 1     | 0.91      | 0.91   | 0.91     | 585     |
| Macro Avg | 0.
