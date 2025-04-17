# Tracking Reuse Tool

A tool for tracking data reuse from CESSDA Service Providers (archives) in academic publications.

## Overview

This R-based tool analyzes how research data from CESSDA (Consortium of European Social Science Data Archives) Service Providers is reused in academic publications indexed by Scopus. It focuses on tracking citations and analyzing patterns of data reuse.

Version 1.2 is optimized for UK Data Service (March 2025).

## Features

- Extracts DOIs of studies from CESSDA data catalogue 
- Tracks citations of these studies in Scopus-indexed publications
- Analyzes reuse patterns including:
  - Distribution of references across datasets
  - Topic classification of cited data
  - Temporal analysis of citations
  - Subject areas of citing publications
  - Types of data creators (universities vs organizations)

## Requirements

- R with the following packages:
  - httr
  - tibble 
  - dplyr
  - tidyverse
  - jsonlite
  - rscopus
  - tidyquery

- Scopus API key (obtain from https://dev.elsevier.com/apikey/manage)

## Outputs

The tool generates several CSV files in a `results` folder:

- `Scopus_CDC_sub.csv` - Overview of all citations
- `group_by_cited_DOI_distribution.csv` - Reference frequency distribution
- `group_by_study_topics.csv` - Topic analysis of cited data
- `group_by_citing_publications.csv` - Publications citing CESSDA data
- `group_by_time_span.csv` - Time between data publication and citation
- And more detailed analysis files

## Citation

If you use this tool, please cite:

Accordino, F., Luzi, D. and Pecoraro, F. (2025), "Challenges in tracking archive's data reuse in social sciences", Digital Library Perspectives, Vol. ahead-of-print No. ahead-of-print. https://doi.org/10.1108/DLP-07-2024-0112

## Author

Filippo Accordino  
Institute for Research on Population and Social Policies - National Research Council, Rome - Italy  
DASSI - Data Archive for Social Sciences in Italy  
f.accordino@irpps.cnr.it  
https://orcid.org/0000-0002-4245-0654

## License

CC BY-NC-SA 4.0