# PIDs Project

## Description
This project performs data manipulation and analysis on a series of Excel files named "report_bookings" using R. It aims to extract specific patterns of data, specifically IDs that match a given pattern, and export these IDs into a CSV file for further analysis or usage. The analysis is scripted in R Markdown, allowing for dynamic execution and report generation with the current date.

## Installation and Setup

### Prerequisites
Ensure you have R and RStudio installed on your system to run R scripts and R Markdown files. This project relies on several R packages for data manipulation, reading Excel files, and other utilities. The required packages are:

- `dplyr`
- `tidyverse`
- `wdman`
- `netstat`
- `xml2`
- `purrr`
- `readr`
- `usethis`
- `dotenv`
- `here`
- `readxl`
- `stringr`

### Setting Up Your Environment
1. Clone or download this repository to your local machine.
2. Open the R Markdown file (`Untitled.Rmd`) in RStudio.
3. Install any missing packages using the provided code snippets at the beginning of the script. The script checks for missing packages and attempts to install them before loading them into the session.

### Data Files
The script expects Excel files named "report_bookings (2).xls" through "report_bookings (6).xls" to be located in your `Downloads` folder. Ensure these files are present before running the script.

## Running the Analysis
To execute the analysis:
1. Open RStudio and set your working directory to the location where the project files are saved. This can be done using the `setwd()` function or through RStudio's graphical interface.
2. Run the R Markdown file. This process will read the Excel files, perform data manipulation to extract and filter data based on specific patterns, and finally, export the filtered IDs to a CSV file named "PIDs.csv".

## Output
After running the script, you will find a CSV file named "PIDs.csv" in your working directory. This file contains the distinct PIDs extracted from the specified column in the Excel files, filtered to match the pattern "730\\d*".

## Note
This README assumes a specific file naming convention and working directory. Adjust the instructions as necessary to fit your project's setup and file organization.
