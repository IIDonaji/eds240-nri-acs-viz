# Visualizing Natural Hazard Risk Patterns

EDS 240— Data Visualization Assignment

# Overview

Visualizations exploring natural hazard risk and demographic exposure using FEMA National Risk Index (NRI) and US Census Bureau American Community Survey (ACS) data.

The goal of this project is to investigate, prepare, and visualize hazard-related data in ways that are effective, responsible, and accessible to a broad audience.

The analysis emphasizes thoughtful visualization choices that align the **data structure, intended message, and target audience**, using the R programming language and the **{ggplot2}** ecosystem.

# Repositroy Structure

```         
── eds240-nri-acs-viz.Rproj
├── HW2.html
├── HW2.pdf
├── HW2.qmd
├── HW3.pdf
├── HW3.qmd
├── LICENSE
└── README.md
```

# Visualizations

## HW2 -FEMA NRI Risk Scores Across US States

Explores how FEMA National Risk Index scores for counties in California compare to those in other states, using county-level NRI data for all 50 US states (no territories).

*Data:* [FEMA NRI](https://www.fema.gov/emergency-managers/practitioners/resilience-analysis-and-planning-tool) (2025 Release)

## HW3 - Climate Hazard Risk Exposure by Race/Ethnicity in California

Examines how climate hazard risk exposure varies across racial and ethnic groups in California by joining county-level NRI scores with ACS demographic estimates.

*Data Sources:* 

- [FEMA NRI](https://www.fema.gov/emergency-managers/practitioners/resilience-analysis-and-planning-tool) (2025 Release) county-level composite risk scores

-   [US Census Bureau American Community Survey (ACS)](https://www.census.gov/programs-surveys/acs) 1-year Estimates (2023)-county-level race and ethnicity population counts

**Racial/ethnic groups included:** White, Black or African American, American Indian and Alaska Native, Asian, Native Hawaiian and Other Pacific Islander, Some Other Race, Two or More Races, Hispanic or Latino

# Data Description

**FEMA National Risk Index (NRI)**

The primary dataset used in this project comes from FEMA's National Risk Index (NRI) for Natural Hazards.

The NRI provides information on community-level risk across 18 natural hazard types at the county and census tract levels in the United States. Risk is defined as the potential for negative impacts resulting from natural hazards and is calculated as:

  **Risk = Expected Annual Loss $\times$ Social Vulnerability $\div$ Community Resilience**
                
For each hazard type and for a composite index, communities are assigned:

-   **Percentile scores** (relative to all other U.S. counties or tracts)

-   **Qualitative risk ratings** (Very Low to Very High)

These metrics allow for comparison of natural hazard risk, vulnerability, and resilience across regions.

**US Census Bureau's American Community Survey (ACS)**

The ACS nationwide, continuous survey collecting detailed information from small subset of population at 1 and 5 year intervals, provides communities timely social, economic, housing and demographic data every year.

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

# Requirements

-   **R Studio**

```
library(tidyverse)
library(tidycensus)
library(here)
library(ggplot2)
```

A [Census API key](https://api.census.gov/data/key_signup.html) is required to download ACS data via `tidycensus`. Once obtained, register it with `tidycensus::census_api_key("YOUR_KEY", install = TRUE)`.

# Audience

Visualizations in this repository are designed for a general, non-technical audience, such as students,while maintaining analytically rigor appropriate for an academic setting.

# Acknowledgments

FEMA for providing the National Risk Index data

Course instructors and materials from [EDS 240](https://eds-240-data-viz.github.io/)
