# Visualizing FEMA NRI Data

EDS 240— Data Visualization Assignment

# Federal Emergency Management Agency's (FEMA) National Risk Index (NRI) & American Community Survey (ACS)

# Overview

This repository contains coursework for a data visualization assignment focused on natural hazards risk in the United States, using data from **FEMA’s National Risk Index (NRI).** The goal of this project is to explore, prepare, and visualize hazard-related data in ways that are effective, responsible, and accessible to a broad audience.

The analysis emphasizes thoughtful visualization choices that align the **data structure, intended message, and target audience**, using the R programming language and the **{ggplot2}** ecosystem.

# Learning Objectives

This project addresses the following learning outcomes:

-   Identify which types of visualizations are most appropriate for specific data types and audiences

-   Prepare and clean data so it is appropriately formatted for visualization

-   Build effective, responsible, accessible, and aesthetically pleasing visualizations

-   Use R, specifically {ggplot2} and related extension packages, to communicate insights from data

# Data Description

**FEMA National Risk Index (NRI)**

The primary dataset used in this project comes from FEMA’s National Risk Index (NRI) for Natural Hazards.

The NRI provides information on community-level risk across 18 natural hazard types at the county and census tract levels in the United States. Risk is defined as the potential for negative impacts resulting from natural hazards and is calculated as:

**Risk = Expected Annual Loss × Social Vulnerability ÷ Community Resilience**

For each hazard type and for a composite index, communities are assigned:

-   **Percentile scores** (relative to all other U.S. counties or tracts)

-   **Qualitative risk ratings** (Very Low to Very High)

These metrics allow for comparison of natural hazard risk, vulnerability, and resilience across regions.

More details about the dataset can be found in [FEMA’s National Risk Index Data Technical Documentation](https://www.fema.gov/sites/default/files/documents/fema_national-risk-index_technical-documentation.pdf).

**US Census Bureau's American Community Survey (ACS)**

The ACS nationwide, continuous survey collecting detailed information from small subset of population at 1 and 5 year intervals, provides communities timely social, economic, housing and demographic data every year. 

# Repositroy Structure

# Methods

The workflow for this project includes:

1.  Data preparation

-   Cleaning and wrangling NRI data

-   Reshaping data for visualization

-   Verifying variable definitions and scales

2.  Exploratory analysis

-   Examining distributions and relationships

-   Identifying patterns in risk, vulnerability, and resilience

3.  Visualization

-   Selecting appropriate chart types for the data and message

-   Designing accessible and interpretable graphics

-   Using **{ggplot2}** and extension packages to enhance clarity and aesthetics

# Tools and Packages

-   **R**

-   **ggplot2**

-   ggplot2 extension packages (e.g., for themes, scales, or annotations)

-   Quarto (.qmd) for reproducible reporting

# Audience

Visualizations in this repository are designed for a general, non-technical audience, such as students,while maintaining analytical rigor appropriate for an academic setting.

# Acknowledgments

FEMA for providing the National Risk Index data

Course instructors and materials from EDS 240
