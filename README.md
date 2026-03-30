# Coffee Survey at Swiss TPH

A data-driven analysis of coffee preferences and consumption at the Swiss TPH.

## Overview

This project contains a survey of 64 respondents examining coffee (and tea) preferences, consumption patterns, and sourcing knowledge at Swiss TPH. The analysis includes demographic breakdowns, taste comparisons between coffee locations, and suggestions for improvement.

## Repository Contents

-   **`coffee_survey.csv`** – Raw survey data from Google Forms (64 responses)
-   **`coffee_survey_analysis_v2.qmd`** – Quarto document with full analysis and visualizations
-   **`coffee_survey_analysis_v2.html`** – Rendered HTML report (self-contained)

## The Analysis

The `.qmd` file is a [Quarto](https://quarto.org/) document that integrates **R code and Markdown text**. Key sections:

-   **Demographics**: Who responded (mostly PhD/Master's students)
-   **Consumption**: Tea vs. coffee preference, daily cups, timing, and reasons
-   **Location Comparison**: Downstairs (cafeteria, fresh milk) vs. Upstairs (machines, powdered milk)
-   **Taste Profiles**: Radar charts and descriptive analysis by location
-   **Sourcing Knowledge**: Most staff don't know where coffee comes from
-   **Improvement Suggestions**: Real milk is the #1 request

### Rendering the Report

To render the Quarto document to HTML:

``` bash
quarto render coffee_survey_analysis_v2.qmd
```

Or, if using RStudio, click **Render** in the editor.

**Prerequisites:** - [Quarto](https://quarto.org/docs/get-started/) - R with libraries: `tidyverse`, `ggpubr`, `ggrepel`, `RColorBrewer`

## Key Findings

-   **75% prefer downstairs coffee** – better taste, creaminess, and balance due to fresh milk
-   **Powdered milk is a dealbreaker** – most upstairs criticism centers on artificial taste
-   **Consistency across roles** – coffee consumption (\~2 cups/day) doesn't correlate with hierarchy
-   **Knowledge gap** – 85% don't know the origin or supplier of coffee beans

## How to Use

1.  **View the analysis**: Open `coffee_survey_analysis_v2.html` in any browser
2.  **Modify & rerender**: Edit the `.qmd` file (R code and text) and run `quarto render`
3.  **Adapt for your institute**: The structure is modular – swap in your own CSV and adjust questions

## Notes

-   **Sample bias**: Heavily skewed toward PhD/Master's students due to survey distribution
-   **Tea data**: Only 9 respondents; too small for robust conclusions but included for completeness

------------------------------------------------------------------------

*Report generated with Quarto, analyzed with R (tidyverse, ggplot2). All code and data in this repo; adapt freely for your institute's beverage survey.*
