Crime Statistics Analysis
===========================

![GitHub](https://img.shields.io/github/license/cbenge509/w203_Final) ![GitHub contributors](https://img.shields.io/github/contributors/cbenge509/w203_Final) ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/cbenge509/w203_Final?include_prereleases)

<img align="right" width="180" src="./images/UCBerkeley.png"/>

#### Team : [Cristopher Benge](https://cbenge509.github.io/) | [Joy First](mailto:jfirst@berkeley.edu) | [Kevin Kory](mailto:knkory92@berkeley.edu)

U.C. Berkeley, Masters in Information & Data Science program - [datascience@berkeley](https://datascience.berkeley.edu/) 

Fall 2019, W203 - Statistics for Data Science - G. Kleeman, PhD <br>
**Final Project**

## Description

This repos contains the R code, Markdown, and final presentation [written in LaTeX] for Lab 3, Final Project in course W203 : Statistics for Data Science @ U.C. Berkeley, School of Information, Graduate Studies.  The analysis consists of a detailed review of crime statistics from 90 North Carolina counties in 1987, review of various regression schemes, and policy suggestions that follow naturally from findings in the data.

#### Highlight of key files included in this repository:

  |File | Description |
  |:----|:------------|
  |[Crime Analysis & Policy Recommendations.pdf](Crime%20Analysis%20&%20Policy%20Recommendations.pdf) | Final analysis report in PDF format.|
  |[first_kory_benge-lab_3.Rmd](first_kory_benge-lab_3.Rmd) | R code file containing the analysis and visuals generation. |
  |[first_kory_benge-lab_3.tex](first_kory_benge-lab_3.tex) | root file for the LaTeX published final document (chapters in subfolders) |
  |[crime_v2.csv](crime_v2.csv) | Raw county-level crime data for North Carolina (circa 1987)  |

#### Notes & Errata:

This solution missed only one key finding in the data: the 10 missing counties in the source data are the lowest populated counties in the state.  This means that the [IID](https://en.wikipedia.org/wiki/Independent_and_identically_distributed_random_variables) assumption has been violated, as the counties under consideration were not randomly selected.

<img src="/images/Model_2_diagnostic_plots.jpg" width="900"/>
<img src="/images/EDA_location_map_correct.jpg" width="900"/>
<img src="/images/EDA_histograms_crmrte.jpg" width="900"/>

License
-------
Licensed under the MIT License. See [LICENSE](LICENSE.txt) file for more details.
