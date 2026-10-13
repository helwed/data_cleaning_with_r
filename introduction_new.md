---
title: "Introduction – Data Cleaning in R"
teaching: 20
exercises: 2
---
:::::::::::::::::::::::::::::::::::::: questions 

- Why is data cleaning an important part of the research workflow?
- How does using R support reproducibility and transparency?
- What kinds of “messiness” do we expect in social science data?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Differentiate data cleaning from data organization.
- Describe how R can be used for reproducible data cleaning.
- Recognize typical data issues in social science datasets.

::::::::::::::::::::::::::::::::::::::::::::::::

## Motivation for using R to clean your data
The Data is the heart of your analysis, but before the actual analysis can begin, you might have to spend a significant amount of time to clean it. This is especially important, if you work with survey data or with any manual annotations (e.g., using abbreviations or codes). 

**Using R for data cleaning helps:**

- Reproducibility & Transparency: Every change you make will be documented in the script and can be published or shared.
- Reusability: The same script can be re-run when you get new or updated data.
- Flexibility: R can handle a wide variety of data types and structures.

## Messy data

In this lesson, we will work with a "messy" version of the SAFI data. It has been changed to include:

- Inconsistent spelling (incl. capitalization) of categorical variables.
- Different codes used for yes/no style questions.
- Missing values and special codes (e.g. -99) for missing data.
- Numeric values that are out of normal ranges.

Before we start to dive into the data itself, let's discuss what experiences with "messy data" you have!

::::::::::::::::::::::::::::::::::::: challenge 

## Challenge 1: Short discussion
In pairs, list typical “messy data” problems that you have seen. We will collect this in the shared document.

:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::: solution 

:::::::::::::::::::::::::::::::::

## Data Cleaning vs. Data Organisation
Data Cleaning vs Data Organization
It is helpful to distinguish between data cleaning and data organization:

Data cleaning focuses on:

- Correcting errors and inconsistencies.
- Handling missing values.
- Making sure values are within normal ranges.
- Standardizing formats (e.g. dates, categories).

Data organization focuses on:

- Structuring files and folders (e.g. data/, scripts/, results/).
- Naming files and variables consistently.
- Documenting metadata (i.e., what each variable means).
- Setting up projects so that code and data are easy to find.

::::::::::::::::::::::::::::::::::::: challenge 

## Challenge 2: Cleaning or Organizing?
For each of the following tasks, decide whether it is primarily data cleaning or data organization:

1. Renaming the column hh_size to household_size.
2. Changing all values "Y", "yes", and "Yes" in a column to a single standardized value "yes".
3. Moving your raw data files into a folder named data/raw/.
4. Replacing all occurrences of -99 in a numeric column with NA to indicate missing data.

Discuss your answers with a neighbor.
:::::::::::::::::::::::::::::::::
:::::::::::::::::::::::: solution 
1. Mostly data organization (improves clarity of variable names).
2. Data cleaning (standardizes categories).
3. Data organization (improves file structure).
4. Data cleaning (handles a special missing-value code).
:::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::: keypoints 

- Data cleaning is a important research activity and should not be an afterthought.
- Scripts in R provide a reproducible documentation of all changes.
- Survey data often contains missing values, inconsistent codes, and typos that must be handled before analysis.

::::::::::::::::::::::::::::::::::::::::::::::::
