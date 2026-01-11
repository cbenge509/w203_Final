# README Redesign Plan

**Date:** 2026-01-11
**Status:** Approved

## Goals

- Primary audience: Academic reviewers evaluating statistical methodology
- Style: Modern GitHub showcase (badges, collapsible sections, polished but rigorous)
- Content level: Substantive summary (~500-800 words for methodology/results)
- Data documentation: Key variables + data quality notes + IID limitation prominently featured

## Structure

1. **Header & Badges** - Clean badges (MIT, R, observations, course), team info, subtitle
2. **Overview** - 2-3 sentence hook describing the study
3. **Key Findings** - Results table with policy implications, recommended model highlighted
4. **Data** (collapsible) - Source, key variables table, cleaning steps, limitations with map
5. **Methodology** (collapsible) - Approach, three model specs table, diagnostics summary with plots
6. **Repository Structure** (collapsible) - Expanded file table
7. **Reproducibility** - Brief, visible code blocks for running analysis
8. **Footer** - Team table, license, closing visualization

## Key Design Decisions

- Results come early (reviewers see findings without scrolling)
- Collapsible sections keep page scannable while allowing deep dives
- IID limitation moves from "Notes & Errata" to dedicated "Data Quality" subsection with warning emoji
- Images integrated contextually (diagnostic plots in Methodology, map in Data)
- Tables throughout for scannability
- Recommended model marked with star emoji

## Content Highlights

### Key Findings Table
| Finding | Effect | Policy Implication |
|:--------|:-------|:-------------------|
| Arrest probability | 1% increase → 0.04% decrease in crime rate | Invest in investigation and clearance rates |
| Conviction probability | 1% increase → 0.04% decrease in crime rate | Support prosecutorial capacity |
| Police per capita | Positive correlation (endogeneity concern) | More police deployed where crime already high |
| Construction wages | Higher wages → lower crime | Economic opportunity reduces crime |
| Young male population | Higher % → higher crime | Target prevention programs to at-risk demographics |

### Model Specifications Table
| Model | Variables | Purpose |
|:------|:----------|:--------|
| Model 1 | prbarr, prbconv, log(polpc), taxpc, wcon | Core deterrence + economic factors |
| Model 2 (recommended) | Model 1 + pctymle, log(pctmin80) | Adds demographic controls |
| Model 3 | Model 2 + wser, wfed, additional controls | Full specification (robustness check) |

### Diagnostics Table
| Assumption | Test | Model 2 Result |
|:-----------|:-----|:---------------|
| Linearity | Residuals vs. Fitted | Pass |
| Normality | Q-Q Plot, Shapiro-Wilk | Pass |
| Homoscedasticity | Breusch-Pagan | Pass |
| Multicollinearity | VIF | Pass (all < 5) |

## Badges to Add
- R version badge
- Dataset size (91 observations)
- Course identifier (W203)

## Images to Integrate
- `EDA_location_map_correct.jpg` - In Data section (shows missing counties)
- `Model_2_diagnostic_plots.jpg` - In Methodology section
- `EDA_histograms_crmrte.jpg` - In footer (closing visual)
