## `BST 270 Individual Project`

**Author:** Addison McGhee (amcghee@hsph.harvard.edu)

**Due Date:** 2022/01/24

### `Introduction`
Welcome to the BST 270 Individual Project!! This project was meant to serve as an exercise in reproducibility, where we the students were tasked with "reproducing" a set of COVID-19 figures the New York Times published on January 12, 2022. These graphs and tables were posted on the [New York Times' COVID-19 dashboard](https://www.nytimes.com/interactive/2020/us/coronavirus-us-cases.html), which is a webpage that is updated daily. 

Our goal was to reproduce the following figures from 2022/01/12:

1. New cases as a function of time (red-shaded line graph with 7-day rolling average)
2. Table of cases and deaths (with 14-day percent change)
3. The map of the United States with county-level data from the previous week ('Hot spots')
4. Table of cases by state (daily avg. cases only)

## `Repo Contents`:

#### `Code`:
This repository contains an R Markdown script (`270_individual_project.Rmd`) with the entire analysis written solely in the [R programming language](https://cran.r-project.org). The .Rmd was knit to .pdf and .html files, which are also present in the repo.

#### `Data`:
Data for cases and deaths can be downloaded from the [NYT GitHub repository](https://github.com/nytimes/covid-19-data). The .Rmd file uses URLs to read and load the data directly from the NYT repository, and so no .csv files were required to be stored in this repo. The data contains county level COVID-19 cases, deaths, daily averages, and daily averages per 100,000 people. Two data sets are used: the first (`us-counties.csv`) contains the cumulative COVID-19 data from the beginning of the pandemic, while the second (`us-counties-2022.csv`) holds data just from 2022.

#### `Images`:
The files `nyt1.png`, `nyt2.png`, `nyt3.png`, `nyt4.png` are images stored as portable network graphics (.png), and these are the actual figures used by the New York Times on 2022/01/12. The numbering (1-4) matches the list of figures above. All of the .png files are necessary to run the .Rmd file. The file `georgia.png` was included to illustrate how not to do data science.

#### `Definitions`:
The following definitions were taken from the NYT GitHub README. These describe the variables used in this project:

`cases:` The number of new cases of Covid-19 reported that day, including both confirmed and probable.

`cases_avg:` The average number of new cases reported over the most recent seven days of data. In other words, the seven-day trailing average.

`cases_avg_per_100k:` The cases_avg per 100,000 people.
deaths: The total number of new deaths from Covid-19 reported that day, including both confirmed and probable.

`deaths_avg:` The average number of new deaths reported over the most recent seven days of data. In other words, the seven-day trailing average.

`deaths_avg_per_100k:` The deaths_avg per 100,000 people.

## `Reproducibility Steps`:
The first step is to download the [R programming language](https://cran.r-project.org) for your specific machine. An appropriate editor is also needed, such as [RStudio](https://www.rstudio.com), to run the .Rmd file. The next step is to load the required libraries ("packages") so that you can use the appropriate functions and datasets for the analysis. The newest version of RStudio will prompt users to download any packages that are not already present. Then, after downloading all the files from this GitHub repo to your "working" directory or folder, you can run the .Rmd script and reproduce these plots and tables.

### Contact
Any questions, comments, and/or concerns should be directed to @Addison-McGhee (amcghee@hsph.harvard.edu).


#### `Attribution`:
"The New York Times. (2021). Coronavirus (Covid-19) Data in the United States. Retrieved 2022/01/19, from https://github.com/nytimes/covid-19-data."


